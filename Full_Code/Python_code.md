# Python Code for the Cition website
```.py
import os
import sqlite3
import jwt
import dotenv
from functools import wraps 
from flask import Flask, render_template, request, redirect, url_for, make_response, session
from mylib import database_worker, encrypt_password, check_password

from datetime import datetime,timedelta


app = Flask(__name__)
app.secret_key = 'ejhvvfwfbjwnwsqwpqqrhphwqnqwdwefhw45678uh23r23313fg2u181gf211dd'

dotenv.load_dotenv()
token_key=os.getenv('TOKEN_ENCRYPTION_KEY')

from functools import wraps
import jwt

def token_required(f):
    @wraps(f)
    def decorated(*args, **kwargs):
        # Check if a token is present in the user's session
        if 'token' not in session:
            print("no token")
            # If no token is present, redirect the user to the login page
            return redirect(url_for('login'))
        try:
            # Attempt to decode the token using the secret key
            print("decoding the token")
            print(session['token'])
            data = jwt.decode(session['token'], token_key, algorithms = ['HS256'])
            print(data)

        except:
            print("wrong token")
            # If the token is invalid, redirect the user to the login page
            return redirect(url_for('login'))

        # If the token is valid, call the decorated function with the original arguments and keyword arguments
        return f(*args, **kwargs)

    # Return the decorated function
    return decorated

def create_database():
    db = database_worker("social_net.db")

    query_user = """Create table if not exists users(
    id INTEGER PRIMARY KEY,
    email TEXT,
    password TEXT,
    city TEXT,
    username TEXT
    )
    """

    query_post = """ CREATE table if not exists posts(
    id INTEGER PRIMARY KEY,
    title VARCHAR(100),
    content TEXT,
    user_id INTEGER,
    publish_date TEXT,
    FOREIGN KEY (user_id) REFERENCES users(id) on delete cascade
   
    )"""
    db.run_save(query_user)
    db.run_save(query_post)
    db.close()

@app.route('/index')
@token_required
def index():  # put application's code here
    return render_template("index.html")

@app.route('/', methods = ['GET', 'POST'])
@app.route('/login', methods = ['GET', 'POST'])
def login():
    msg=''
    if request.method == 'POST':
        email = request.form['email']
        passwd = request.form['passwd']
        db = database_worker("social_net.db")
        user = db.search(f"SELECT * from users where email ='{email}'")
        if user:
            print("passed")
            user = user[0]  # cause search returns a list
            id, email_db, hashed, city, uname = user
            if check_password(hashed_password = hashed, user_password = passwd):
                response = make_response(redirect(url_for('profile',user_id = id)))
                response.set_cookie('user.id', f"{id}")
                token = jwt.encode({'user_id': id, 'exp': datetime.utcnow() + timedelta(minutes=30)}, token_key, algorithm = 'HS256')
                session['token'] = token
                return response
        else:
            msg="user does not exist"

    return render_template("login.html",message=msg)


@app.route('/logout')
def logout():
    response = make_response(redirect('login'))
    response.set_cookie("user_id", "", expires = 0)
    session.pop('token', None)

    return response

@app.route('/register', methods=['GET', 'POST'])
def register():
    if request.method == 'POST':
        email = request.form['email']
        password = request.form['password']
        city = request.form['city']
        username = request.form['username']
        # Generate hashed password
        hashed_password = encrypt_password(password)
        # Insert user data into database
        conn = sqlite3.connect('social_net.db')
        c = conn.cursor()
        c.execute("INSERT INTO users (email, password, city, username) VALUES (?, ?, ?, ?)", (email, hashed_password, city, username))
        conn.commit()
        conn.close()
        # Redirect user to login page
        return redirect(url_for("login"))
    return render_template('register.html')


@app.route('/user/<user_id>', methods = ['GET', 'POST'])
@token_required
def profile(user_id: int):
    if not request.cookies.get('user.id'):
        return redirect(url_for('login'))
    else:
        db = database_worker("social_net.db")
        current_user_id = request.cookies.get('user.id')  # get the ID of the currently logged in user
        if request.method == 'POST':
            title = request.form['title']
            content = request.form['content']
            now=datetime.now()
            today = now.strftime("%d/%m/%Y")
            if len(title) > 0 and len(content) > 0 and str(user_id) == current_user_id:  # check if the post is being made by the logged in user
                new_post = f"Insert into posts (title,content,user_id,publish_date) values('{title}','{content}','{user_id}','{today}')"
                db.run_save(query = new_post)
                return redirect(url_for('profile', user_id = user_id))
        users, posts = None, None
        user = db.search(f"SELECT * from users where id={user_id}")
        if user:
            posts = db.search(f"select * from posts where user_id={user_id}")
            user = user[0]  # remember search returns a list (should be one user so...

        return render_template("profile.html", user = user, posts = posts, current_user_id=int(current_user_id))


@app.route('/delete_profile')
@token_required
def delete_profile():
    if not request.cookies.get('user.id'):
        return redirect(url_for('login'))
    else:
        db = database_worker("social_net.db")
        current_user_id = request.cookies.get('user.id')  # get the ID of the currently logged in user
        query=f"Delete from users where id={current_user_id}"
        db.run_save(query = query)
        return redirect('login')


@app.route('/cities', methods=["GET", "POST"])
@token_required
def cities():
    db = database_worker("social_net.db")
    all_cities = db.search("select * from cities")
    return render_template("cities.html", cities=all_cities)


@app.route("/city/<city_name>")
def get_city(city_name):
    db = database_worker("social_net.db")
    city_data = db.search(f"select * from cities where name='{city_name}'")
    return render_template("city.html", city=city_data[0])

@app.route('/my_profile')
def my_profile():
    user_id = session.get('user_id') or request.cookies.get('user.id')
    if not user_id:
        return redirect(url_for('login'))

    return redirect(url_for('profile', user_id=user_id))

@app.route('/users')
@token_required
def users():
    # Checks if the user is authenticated by checking if the user.id cookie exists
    if request.cookies.get('user.id'):
        db = database_worker("social_net.db") # Creates a database worker object to perform SQL queries on the "social_net.db" database
        all_users = db.search("SELECT * FROM users")# Selects all users from the "users" table
        db.close()# Closes the database connection
        city = request.args.get('city')# Gets the city chosen from the option bar (if any)
        search_query = request.args.get('search_query')
        # Filters the list of all_users to only include those that contain the search query (case insensitive)
        # if a search query is provided through the search bar filter
        if search_query:
            all_users = [user for user in all_users if search_query.lower() in user[4].lower()]
        return render_template("user.html", users = all_users, city = city)
    else:
        return redirect("login")


@app.route('/posts')
@token_required
def posts():
    if request.cookies.get('user.id'):
        db = database_worker("social_net.db")
        all_posts = db.search("SELECT * FROM posts")
        db.close()
        return render_template("posts.html", posts = all_posts)
    else:
        return redirect("login")

#
# print("creating database")
# create_database()
# print("populating the users table")
#populate_db()
if __name__ == '__main__':
    app.run()
    ```
