# Citio social network
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/Project4pictureDreamAi.jpg)


Fig.1 shows the picture created for Citio Dream AI[^1] generated on the prompt Create an image of people taking pictures of local japanese shops and shrines on their phiones and clouds representing their social media posts about it.
## 1. [Criteria A: Planning](#criteria-a-planning)
1.1. [Definition of the problem](#problem-definition)

1.2. [Success Criteria](#success-criteria)

1.3. [Design Statement](#design-statement)

1.4. [Rationale for proposed solution](#rationale-for-proposed-solution)
## 2. [Criteria B: Design](#criteria-b-design)
2.1[System Diagram](#system-diagram)

2.2. [Wireframe Diagram](#wireframe-diagram)

2.3. [ER Diagram](#er-diagram)

2.4. [UML Diagram](#uml-diagram)

2.5. [Flow Diagram](#flow-diagram)

2.6. [Test plan](#test-plan)

2.7. [Record of tasks](#record-of-tasks)

## 3. [Criteria C: Development](#criteria-c-development)
3.1.[Tools and techniques used](#tools-and-techniques-used)

3.2. [Sources](#sources)

3.3[Development](#development)

## 4. [Criteria D: Functionality](#criteria-d-functionality)
 
4.1 [SNS Video](#video-showcase)

4.2 [Appendix](#appendix)
# Criteria A: Planning
## Problem Definition
Being in love with exploring small local shops and restaurants, visiting tourist attractions, and everything else that a city has to offer, I have always faced the big challenge of finding them, as they can be hardly found on google maps where only a few places and creators gain exposure, eliminating smaller local shops and restaurants due to their lack of marketing. Another big problem is not having a place where my friends could see only the recipes I upload, so that they could enjoy my exceptional cullinary skills. Current social networks gave these smaller businesses more exposure, but a user has to put great effort to narrow the search only to relevant local places and creators located in their city, and can not find specific creators located in their city. If an adequate solution is not presented soon, these smaller businesses will close due to a lack of traffic, resulting in market concentration, which in turn would hurt the economy and tourism of cities. This problem definition was established with the help of the data gathered through questionnaires.(referred to in the appendix)

## Proposed Solution
To provide more exposure for the local places and prevent them running out of business, I have decided to make a web applicaton that would serve as a place where people could connect with others through sharing interesting local places, culinary expiriences and astonsihing nature that one city has to offer.

### Why Web Application?
Web applications are more adequate when developing a social network like the one I am making because it allows easier access and sharing of information across multiple devices without the need for downloading and installing an application. Users can simply access the website through a web browser on their desktop or mobile devices. THis increases the potential audience size as makes it easier for users to share their experiences with others. Lastly, a web applications can be maintained easily and can be optimized for search engines, making it easier for new users to discover and join the social network.

### Why Python?
Python contains many versatile features, which make it a better choice compared to other languages, for example PHP[^2]. Python's Flask framework is ideal for developing social network websites due to its lightweight and flexible nature [^3]. Flask's simplicity and ease of use make it an excellent choice for this project, allowing developers to focus on the website's core features and functionality. It also offers a range of libraries and extensions, making it easier to implement complex features such as authentication and database connectivity, when compared to its competitors such as PHP or ruby [^4]. With Python's object-oriented programming, developers can write code that is easy to read, modify, and maintain, which is essential when creating a complex web application such as a social network website. Additionally, Python has an active community of developers who offer support and resources, making it easier to learn and develop with the language.

### Why SQL?
To store the vast amounts of data needed for a social network website, a reliable and efficient database is essential. While non-SQL databases can be an option, SQL databases offer several advantages that make them better suited for this purpose. The main advantage of SQL databases is their ability to handle large amounts of data efficiently, thanks to their relational structure[^5]. The relational structure of SQL databases makes it easier to manage and query data, as it is stored in tables. This feature also ensures that data is consistent and accurate, as it is subject to strong data integrity constraints[^6]. With all the data that is being stored for this social network website, an SQL database is essential to ensure efficient data handling and management.

### Why HTML?
HTML is the standard markup language used to create web pages and it provides the structure and content of a website[^7]. Compared to other alternatives such as Flash, HTML is more widely supported, making it a better choice for cross-platform compatibility[^8]. Additionally, HTML is more search engine friendly than other technologies such as JavaScript, which can lead to better search engine rankings[^9].

## Design Statement
I will design a new creative social network that will allow users to share their reviews of the small local places. The development will be done using the software Flask framework in Python, CSS and HTML. It will take around 5 weeks to develop and will be evaluated according to the success criteria stated below by the client.

## Success Criteria
1. The social network website will provide a secure login and registration system. 
>[ Another big problem is not having a place where my friends could see only the recipes I upload]
2. The social network website will allow users to post reviews of the local places, containing title, date, and content. 
>[I have always faced the big challenge of finding them, as they can be hardly found on google maps where only a few gain exposure]
3. The social network website will have a feature to display all users and the city about which they post. 
>[user has to put great effort to narrow the search only to relevant local places and creators located in their city]
4. The social network website will have an option to choose a specific city which you are interested in through a filter or use a username search filter, and see only relevant content creators. 
>[user has to put great effort to narrow the search only to relevant local places located in their city and can not find specific creators located in their city.]
5. The social network website will to have a feature to see all reviews posted by a specific user, by selecting their profile. 
>[where only a few palces and creators gain exposure, eliminating smaller local shops and restaurants due to their lack of marketing]
6. The social network website will have an interactive option display available cities which user could explore, with an option to learn about each one, by simply clicking at the picture of it. 
>[ a specific city which you are interested in & these smaller businesses will close due to a lack of traffic]

# Criteria B: Design
## System Diagram
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/SystemDiagramPr2_v2.png)
Fig.2 shows the system diagram of the social network website
## Wireframe Diagram
![]()
Fig.3 Shows the wireframe diagram of the Social network website.
## ER Diagram
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/erDiagramProject4Final.png)
Fig.4 shows database structure of the social network website
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/user%20databse.png)
Fig.5 shows user database of the social network website, presented in the ER diagram (data provided in the example is not actual data gathered from any of the users.)
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/post%20database.png)
Fig.6 shows post database of social network website, presented in the ER diagram (data provided in the example is not actual data gathered from any of the users.)
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/project4databaseCity.png)
Fig.7 shows the city database of the social network website, presneted in the ER diagram (Fig.4). (Examples provided are the cities currently available in the Citio SNS.)
## UML Diagram
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/Screenshot%202023-04-21%20at%2023.48.39.png)
Fig. 7 shows the class used for manipulating database, used for the website application 
## Flow Diagram
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/project4_flowch1_register.png)
Fig.8 Shows the flow diagram for the registration system of the Citio social network website
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/User%20list%20feature%20flow%20diagram%20-%20Flowchart.png)
Fig.9 Shows a flow diagram for the user list feature and its select city and search by username filters. 
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/flow%20diagram%20for%20the%20profile%20feature%20-%20Flowchart.png)
Fig.10 Shows a flow diagram representing the feature that allows to view a specific user profile and if it is the profile of the user logged in it allows him to upload a post.
## Test plan
|Test Number|Description|Test Type| Target|Procedure|Expected Outcome|
|-----------|-----------|--------|-----------|-----------------|----|
|1|Account registration system|Unit testing|Have a fully functional registration system that checks if the proper values are inputed in the email and password fields|(1) Run Project_4.py (2) Click the register button on the login screen (3) Input data on all the fields (4) After filling in all the fields create an account (5) Try to login with the new account too see if it exists now| After following the procedure, a user should be able to login using the credentials of the newly created account|
|2|User list inspecting |Unit testing| be able to access the user list and see all the registered users and their username and the city which they post about.|(1)Run Project_4.py(2)Login using adequate credentials. (3)Choose the "see all users" option from the navigation bar.(4)Check if the redirected page shows a table containing: id,username, and city for each user| User is able to access the user list from the main menu and will be able to see all the citio users| 
|3|Accesing a specific user's profile from the user list|Integration testing| Access a specific user's profile  by choosing it from the user list|(1)Run Project_4.py(2)Login using adequate credentials. (3)Choose the "see all users" option from the navigation bar. (4) Choose a desired user and click on its nickname to get redirected to his profile. (5) Check if his profile and posts  (if there are any) are displayed successfully| A user can choose to view a specific creator profile that he is interested in.|
|4|Finding a specific user through filter options in the user table|Integration testing|Find a user through username search or by choosing a specific city of interest |(1)Run Project_4.py(2)Login using adequate credentials. (3)Choose the "see all users" option from the navigation bar. (4) Choose a city and see if only users from that city appear in the user table. (5) Now type a certain username or a part of it and see if only adequate users appear | Both filter function work and are properly integrated with the user table database and main menu|
|5|Code practices around html and python, regarding usage of loops and their nesting  |Code Review| Replace repeating funcitons and features using better coding practices by using loops, and make the code more efficient by nesting loops.|(1) Review Project_4.py python code and html code t see any repetitive parts. (2) Create an algortihm that would replace the repetitive part using loops and nesting them if neccesary. (3) Replace the old repetitive code and connect new algorithm and html code to the main SNS code | The code now uses loops for the profile accessing, and for the learn about city feature.| 
|6| Commenting on complexed code practices |Code Review| Adding comments that would explain the usage of more complex programming tools and algorithms to help future potential developers| (1) Review the python Project_4.py code and focus on the mkore complexed algortihms and routes that have a unique features (2) Add a comment explaining their usage and function in the code| The code is easier to understand and is more open for future co-development|
Table 1:
<br>
Shows the test plan containing information about testing done for this application. There are 3 different types of tests presented in the test plan which are unit test(to test one part of the program), integration test(to test the cooperation of different parts) and code review(to check the quality of code). Table shows description, steps to follow, and expected output with a goal to help user understand the process better.



## Record of Tasks
| Task No | Planned Action   | Design Cycle                                            | Planned Outcome                                                                                                 | Time estimate | Target completion date | Criterion |
|---------|--------------------------------------------------------|-------|-----------------------------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| 1       | Write the Problem Definition |Planning| Write a precise problem definition that identifies a problem, consequences of it, and a clear solution that is being proposed    | 25min         | April 7th    | A         |
| 2  |  Write down design statement |Planning| Have a first version of the design statement done  |  10 min | April 9th  |  A   |
| 3  |  Write down first success criteria established during the first user meeting|Planning |Have a first version of success criteria inspired by potential future users. Their opinions and preferences were gathered through a questionire  | 40min  | April 10th  |  A   |
|4| Write a proposed solution| Planning|Propose a solution for the Web application| 15 min| April 11th| A |
| 5 | Write down rationale for the proposed solution |Planning|  Have the firt version of rationale written down  | 45 min  | April 13th  |  A   |
| 6 | Rewrite success criteria initially stated|Planning | Have a clearer version of success criteria| 15 min  |  April 13th  | A|
| 7  | Add table of content| Planning |  Add table of content at the top of the file |20 min| April 15th   |   A  |
|  8 | Create an ER diagram|Design  |  Have an database structure representation for the social network website | 25 min  |  April 15th |   B  |
| 9 |  Create first version of SNS user interface welcome screen|Development | Have user interface for the starting screen using CSS and HTML style features  |50 min  |  April 15th |  C   |
|  10| Create System diagram for SNS| Design| Have a first version of system diagram done and ready to be presented to the client | 30 min  | April 16th  | B |
| 11|   Create functional registration system and have a first version UI for it  created|Development |  Have a functional registration system for the SNS | 35 min    | April 17th    |C
|  12 | Create a active password policy check for the login feature|Development  | Have a visual presentation showing if the password policy has been met or not  | 25 min | April 18th    | C
|  13 | Work on flow diargam for the registration system of the SNS and the users list of the SNS| Design  | Have flow diagram that represnets registration system and the user list done  | 55 min  |  April 18th |   B  |
|  14 |  Work on the user list UI and list information| Development | Redo initial UI for the user list webpage and add city information to the user informations displayed in the list  |  40 min | April 19th  |   C  |
|   15| Create the second version of the system diagram| Design  |  Create a more accurate version of a system diagram | 20 min  | April 19th  | B |
| 16  |  Create a questionaire upload client questionaires in the appendix section |Evaluation |  Have two client questionaires uploaded to the appendix | 25 min  | April 20th  |  D  |
| 17  | Add a base template options menu to all the pages| Development | Have an options menu containg logout, user list, read articles...  | 30 min  |April 21st   |C     |
|  18 | Create a UML diagram for the web aplication| Design | Have a Uml Diagram fimished for the SNS  | 15 min  | April 21st  |  B   |
| 19  | Update the test plan and add 2nd integration test, testing user list feature of the website| Testing  | Have a written test about user list feature  |  10 min | April 22nd  |  B   |
|20   | Test accesing the user list from the main menu page|  Testing| Update the test plan with integration test relating allowing registered user to acces the table containing users of citio| 15 min  |  April 22 | B    |
|  21 | Test accesing a specific user from the user list feature.|Testing | Update the test plan with integration test relating the feature that check a specific account from the user list  |  15 min | April 22nd  |  B   |
|  22 |  Creating new UI for the register, login, and home page of the website|Development | Have more modern UI for the mentioned pages   | 40 min  | April 24th  |   C  |
|   23| Add a filter by city option for the user table | Development |  Have a functioning feature to select the city of interest and see only relevant content creators | 20 min |  April 24th |  C   |
|   24| Add a search bar option for the user table |Development| Have a functioning username search abr that will allow searching for a desried user/s fromthe user table  | 40 min  | April 24th  |  C   |
|   25| Do integration testing on the newly added filter options and the user list display option|Testing  | See if all filter options work properly  | 10 min  | April 24th  |  B   |
|   26| Add a access token to the website |Development |  Secure that users can not access the website options unless they are logged in | 35 min  |April 25th |C  |     
|   27|  Crate a feature to allow users to explore and learn about cities provided in Citio application| Development | Have an option to learn about cities offered in Citio by clicking at the picture of them  | 1h 45 min | April 26th  |  C  |
|   28|  Create a flow diagram for the the user profile page| Design |Visually present the feature of viewing a specific profile thrrough a flow diagram   | 45 min  | April 26th  |   B  |
|  29 |  Write down the development process of fullfilling the success criteria 1 (login/register)|  Development|  Show the development process and computetional thinking behind the login / register options | 40 min  | April 26th  |  C   |
|  30 | Create a final version of the ER diagram that incldues new city informations in the database |Design |  A new ER diagram shows most recent databse structure adequatelly |  10 min | April 26th  |   B  |
|  31 | Create a city database |Development  | Have a database that conntains names, pcitures, desctiptions, fun facts. about cities from Citio  |  25min | April 26th  |   C  |
|  32 | Run code review testing for potential loops and loop nesting and see if any complex algorithms used need a comment to explain them to potential co-developers |Testing | Have a more efficient code of higher quality and better coding practices that would make future co-development easier  | 25 min   | April 26th  |  B   |
| 33|Add a delete account option to the Social network website |Development | Be able to delete your account | 15 min| April 28th|C |
|34|Write down a development process for fulfilling success criteria 2 (Posting reviews)|Development | Show the developing process of the python code that fulfilled the 2nd success criteria stated in the success criteria stated above| 30 min |28th April |C |
| | | | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |


Table 2:	
<br>
Record of Task-:shows the planning and working process throughout the project. This includes: programming, documentation, client's meetings, and other process from the start of the project to the due date. Table contains order, description, Planned Outcome, Design Cycle, Time Estimate, Target Completion, Criteria
# Criteria C: Development
## Tools and techniques used
1. Manipulating SQLite Database
2. Variables
3. For loops
4. If statements
5. Functions
6. Password Hashing
7. Nesting loops
8. HTML template usage
9. JWT session token usage
10. Cookie usage
11. CSS web design 

## Sources
1. “Beautiful CSS Buttons Examples - CSS Scan.” 92 Beautiful CSS Buttons Examples - CSS Scan, https://getcssscan.com/css-buttons-examples. 
2. “Flask HTTP Methods, Handle GET &amp; Post Requests.” GeeksforGeeks, GeeksforGeeks, 2 Feb. 2023, https://www.geeksforgeeks.org/flask-http-methods-handle-get-post-requests/. 
3. “Cirrus CSS.” Cirrus, https://www.cirrus-ui.com/buttons/basics. 
4. Auth0. “JSON Web Tokens.” Auth0 Docs, https://auth0.com/docs/secure/tokens/json-web-tokens. 
5. “How to - Search Bar.” How To Create a Search Bar, https://www.w3schools.com/howto/howto_css_searchbar.asp. 

## Development
#### Design aspect of the social network 
```.html

<style>
    body {
        font-family: Arial, sans-serif;
        font-size: 18px;
        margin: 0;
        padding: 0;
    }

    .navbar {
        overflow: hidden;
        background-color: #79bcff;
        border-radius: 30px 30px 30px 30px;
        margin-bottom: 20px;
    }

    .navbar a {
        float: left;
        display: block;
        color: #fff;
        text-align: center;
        padding: 14px 18px;
        text-decoration: none;
        font-size: 18px;
        font-weight: bold;
        letter-spacing: 2px;
        margin-right: 10px;
    }

    .navbar a:hover {
        background-color: #394bf6;
    }

    .container {
        display: flex;
        align-items: center;
        justify-content: center;
        margin: 0 auto;
        max-width: 800px;
        background-color: #fff;
        border-radius: 30px 30px 30px 30px;
        padding: 20px;
    }

    .options {
        display: flex;
        flex-direction: column;
        margin-left: 20px;
    }

    .options a {
        display: block;
        color: #333;
        text-decoration: none;
        margin-bottom: 10px;
        font-size: 20px;
        padding: 10px 20px;
        border-radius: 10px;
        background-color: #9ecbff;
        transition: background-color 0.3s ease;
    }

    .options a:hover {
        background-color: #6ca2d8;
        color: #fff;
    }

    .image {
        border-radius: 30px 0 0 30px;
        overflow: hidden;
        width: 600px;
        height: 400px;
    }

    .image img {
        width: 100%;
        height: 100%;
        object-fit: cover;
    }
</style>
```
Fig.11 Shows the style features used in the bas template design of social network. The idea for a base template came from the patern recognition of the similar goals for final designs of differnet features throughout the social network. Instead of rewriting the template every time, I create a base template used for colors of all pages in social network website. In terms of web design, using a light blue color scheme can help create a sense of tranquility and trustworthiness, making it a good choice for websites related to health, finance, or technology. [^10]



```.html
<div class="navbar">
    <a href="{{ url_for('index') }}">Home</a>
    <a href="{{ url_for('users') }}">Users</a>
    <a href="{{ url_for('cities') }}">Cities</a>
    <a href="{{ url_for('posts') }}">Posts</a>
    <a href="{{ url_for('my_profile') }}">Your profile</a>
    <a href="{{ url_for('logout') }}">Logout</a>
    <a href="{{ url_for("delete_profile") }}">Delete the account</a>
</div>
```
Fig.12 Another patern that I have recognized was that I needed certain features one click away, regardless of what webpage of the website I was on. This is why I created a navigation bar that is located within the base template, allowing access to certain featrures from whicever page user is currently on.
### Success Criteria 1: The social network website will provide a  secure login and registration system. 
#### Password encryption
```.py
from passlib.context import CryptContext

pwd_config = CryptContext(schemes = ["pbkdf2_sha256"],
                          default = "pbkdf2_sha256",
                          pbkdf2_sha256__default_rounds = 30000
                          )
```
Fig. 13 shows the process and encryption method used for the password hashing for the Social network website. To prevent any serious harm in the case of data leaking, where if the same password is used in multiple places, intruder can use that and the email for other web services, hurting the user in the process.
```.py
# this function receives unsafe password and returns the hashed password
def encrypt_password(user_passowrd):
    return pwd_config.encrypt(user_passowrd)

```
Fig. 14 shows method which calls the previously metnioned process of encryotion.
In order to fulfill client's request for the website, a secure data storing is neccesary and it allows privacy of the user to stay at a desired level.

#### Regsitration System
```.py
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
```
Fig. 15 shows

#### Login System
```.py
 if request.method == 'POST':
        email = request.form['email']
        passwd = request.form['passwd']
        db = database_worker("social_net.db")
        user = db.search(f"SELECT * from users where email ='{email}'
```
Fig. 16 shows
```.py
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
```
Fig. 17 shows

### Success Criteria 2: The social network website will allow users to post reviews of the local places, containing title, date, and content. 
```.py
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

```
Fig. 18 shows

### Success Criteria 3: The social network website will have a feature to display all users and the city about which they post. 
```.py
@app.route('/users')
@token_required
```
```.py
def users():
    # Checks if the user is authenticated by checking if the user.id cookie exists
    if request.cookies.get('user.id'):
        db = database_worker("social_net.db") # Creates a database worker object to perform SQL queries on the "social_net.db" database
        all_users = db.search("SELECT * FROM users")# Selects all users from the "users" table
        db.close()# Closes the database connection
        
```
Fig. 19 shows

### Success Criteria 4: The social network website will have an option to choose a specific city which you are interested in through a filter or use a username search filter, and see only relevant content creators. 
```.py
city = request.args.get('city')# Gets the city chosen from the option bar (if any)
        search_query = request.args.get('search_query')
        # Filters the list of all_users to only include those that contain the search query (case insensitive)
        # if a search query is provided through the search bar filter
        if search_query:
            all_users = [user for user in all_users if search_query.lower() in user[4].lower()]
        return render_template("user.html", users = all_users, city = city)
    else:
        return redirect("login")
```
Fig. 20 shows

### Success Criteria 5: The social network website will to have a feature to see all reviews posted by a specific user, by selecting their profile. 
```.py
      users, posts = None, None
        user = db.search(f"SELECT * from users where id={user_id}")
        if user:
            posts = db.search(f"select * from posts where user_id={user_id}")
            user = user[0]  # remember search returns a list (should be one user so...

        return render_template("profile.html", user = user, posts = posts, current_user_id=int(current_user_id))
```
Fig. 19 shows

### Success Criteria 6: The social network website will have an interactive option display available cities which user could explore, with an option to learn about each one, by simply clicking at the picture of it. 
```.py
@app.route('/cities', methods=["GET", "POST"])
@token_required
def cities():
    db = database_worker("social_net.db")
    all_cities = db.search("select * from cities")
    return render_template("cities.html", cities=all_cities)

```
Fig. 21 shows

```.py
@app.route("/city/<city_name>")
def get_city(city_name):
    db = database_worker("social_net.db")
    city_data = db.search(f"select * from cities where name='{city_name}'")
    return render_template("city.html", city=city_data[0])

```
Fig. 22 shows


# Criteria D: Functionality
## Video showcase
# Appendix
### Filled out questionaire Tester 1
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/user_questionaire1.png)
### Filled out questionaire Tester 2
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/user_questionaire2.png)
# Works cited
[^1]: Dream AI generated image (https://Project4pictureDreamAi.jpg)
[^2]: Sengar, Ritesh. “Python vs PHP: Which Is Better for Web Development?” Hackernoon, 7 Jan. 2021, hackernoon.com/python-vs-php-which-is-better-for-web-development-cj1236mj. 
[^3]: "Welcome to Flask." Flask Documentation, 15 Jan. 2023, flask.palletsprojects.com/en/2.1.x/. 
[^4]: Grinberg, Miguel. Flask Web Development: Developing Web Applications with Python. 2nd ed., O'Reilly Media, Inc., 2018. 
[^5]: “What Is a Database?” Oracle, https://www.oracle.com/database/what-is-database/. 
[^6]: "What is SQL?" W3Schools, W3Schools, https://www.w3schools.com/sql/
[^7]: "HTML Introduction." W3Schools, W3Schools, https://www.w3schools.com/html/html_intro.asp
[^8]: "Flash vs. HTML5." Digital.gov, 17 Dec. 2015, https://digital.gov/resources/flash-vs-html5/.
[^9]: "Why You Need an SEO-Friendly Website." SEO Werkz, 11 Jan. 2022, https://www.seowerkz.com/why-you-need-an-seo-friendly-website/.
[^10]: https://www.smashingmagazine.com/2010/01/color-theory-for-designers-part-1-the-meaning-of-color/
