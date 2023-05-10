# Citio social network
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/dream_TradingCard%20(1).jpg)


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
## 5. [Criteria E: Evaluation](#criteria-e-evaluation)
5.1 [Table of Evaluation](#evaluation-table)
## [Appendix](#appendix)
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
1. The social network website will provide a secure login and registration s[
](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/erDiagramProject4Final.png)ystem. 
>[ Another big problem is not having a place where my friends could see only the recipes I upload]
2. The social network website will allow users to post reviews of the local places, containing title, date, and content. 
>[I have always faced the big challenge of finding them, as they can be hardly found on google maps where only a few gain exposure]
3. The social network website will have a feature to display all users, their contact email, and the city about which they post. 
>[user has to put great effort to narrow the search only to relevant local places and creators located in their city]
4. The social network website will have an option to choose a specific city which you are interested in through a filter or use a username search filter, and see only relevant content creators. 
>[user has to put great effort to narrow the search only to relevant local places located in their city and can not find specific creators located in their city.]
5. The social network website will to have a feature to see all reviews posted by a specific user, by selecting their profile. 
>[where only a few palces and creators gain exposure, eliminating smaller local shops and restaurants due to their lack of marketing]
6. The social network website will have an interactive option display available cities which user could explore, with an option to learn about each one, by simply clicking at the picture of it. 
>[ a specific city which you are interested in & these smaller businesses will close due to a lack of traffic]

# Criteria B: Design
## System Diagram
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/Project_4%20System%20DiagramLAST.png)
Fig.2 shows the system diagram of the social network website
## Wireframe Diagram
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/WIREFRAMEFINALL.png)
Fig.3 Shows the wireframe diagram of the Social network website. All of the main pages are connected through the navigation bar (indicated with red arrows), which was part of the base template used for the Citio website.
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
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/Screenshot%202023-05-10%20at%2011.54.43.png)
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
|1|Account registration system|Unit testing|Have a fully functional registration system that checks if the proper values are inputed in the email and password fields|(1) Run Project_4.py (2) Click the register button on the login screen (3) Input a username: TesterSNS, email: testersns@gmail.com,password:QwErTy and city: Karuizawa that will be used for this tester account(4) After filling in all the fields create an account (5) Try to login with the new account too see if it exists now| After following the procedure, a user should be able to login using the credentials of the newly created account|
|2|User list inspecting |Unit testing| be able to access the user list and see all the registered users and their username and the city which they post about.|(1)Run Project_4.py(2)Login using adequate credentials for the tester account created in the test no.1. (3)Choose the "see all users" option from the navigation bar.(4)Check if the redirected page shows a table containing: id,username, and city for each user| User is able to access the user list from the main menu and will be able to see all the citio users| 
|3|Accesing a specific user's profile from the user list|Integration testing| Access a specific user's profile  by choosing it from the user list|(1)Run Project_4.py(2)Login using adequate credentials for the tester account created in the test no.1. (3)Choose the "see all users" option from the navigation bar. (4) Choose a desired user and click on its nickname to get redirected to his profile. (5) Check if his profile and posts  (if there are any) are displayed successfully| A user can choose to view a specific creator profile that he is interested in.|
|4|Finding a specific user through filter options in the user table|Integration testing|Find a user through username search or by choosing a specific city of interest |(1)Run Project_4.py(2)Login using adequate credentials for the tester account created intest no.1. (3)Choose the "see all users" option from the navigation bar. (4) Choose a city and see if only users from that city appear in the user table. (5) Now type a certain username or a part of it and see if only adequate users appear | Both filter function work and are properly integrated with the user table database and main menu|
|5|Code practices around html and python, regarding usage of loops and their nesting  |Code Review| Replace repeating funcitons and features using better coding practices by using loops, and make the code more efficient by nesting loops.|(1) Review Project_4.py python code and html code t see any repetitive parts. (2) Create an algortihm that would replace the repetitive part using loops and nesting them if neccesary. (3) Replace the old repetitive code and connect new algorithm and html code to the main SNS code | The code now uses loops for the profile accessing, and for the learn about city feature.| 
|6| Commenting on complexed code practices |Code Review| Adding comments that would explain the usage of more complex programming tools and algorithms to help future potential developers| (1) Review the python Project_4.py code and focus on the mkore complexed algortihms and routes that have a unique features (2) Add a comment explaining their usage and function in the code| The code is easier to understand and is more open for future co-development|


Table 1:
<br>
Shows the test plan containing information about testing done for this application. There are 3 different types of tests presented in the test plan which are unit test(to test one part of the program), integration test(to test the cooperation of different parts) and code review(to check the quality of code). Table shows description, steps to follow, and expected output with a goal to help user understand the process better.



## Record of Tasks
| Task No | Planned Action                                              | Planned Outcome                                                                                                 | Time estimate | Target completion date | Criterion |
|---------|-------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| 1       | Write the Problem Definition (Planning) | Write a precise problem definition that identifies a problem, consequences of it, and a clear solution that is being proposed    | 25min         | April 7th    | A         |
| 2  |  Write down design statement (Planning)| Have a first version of the design statement done  |  10 min | April 9th  |  A   |
| 3  |  Write down first success criteria established during the first user meeting(Planning) |Have a first version of success criteria inspired by potential future users. Their opinions and preferences were gathered through a questionire  | 40min  | April 10th  |  A   |
|4| Write a proposed solution (Planning)|Propose a solution for the Web application| 15 min| April 11th| A |
| 5 | Write down rationale for the proposed solution (Planning)|  Have the firt version of rationale written down  | 45 min  | April 13th  |  A   |
| 6 | Rewrite success criteria initially stated(Planning) | Have a clearer version of success criteria| 15 min  |  April 13th  | A|
| 7  | Add table of content (Planning) |  Add table of content at the top of the file |20 min| April 15th   |   A  |
|  8 | Create an ER diagram (Design)  |  Have an database structure representation for the social network website | 25 min  |  April 15th |   B  |
| 9 |  Create first version of SNS user interface welcome screen (Development) | Have user interface for the starting screen using CSS and HTML style features  |50 min  |  April 15th |  C   |
|  10| Create System diagram for SNS and create the wireframe diagram for the Citio webite (Design)| Have a first version of system diagram and wireframe that shows the structure of the website done and ready to be presented to the client | 30 min  | April 16th  | B |
| 11|   Create functional registration system and have a first version UI for it  created (Development) |  Have a functional registration system for the SNS | 35 min    | April 17th    |C
|  12 | Create a active password policy check for the login feature (Development)  | Have a visual presentation showing if the password policy has been met or not  | 25 min | April 18th    | C
|  13 | Work on flow diargam for the registration system of the SNS and the users list of the SNS (Design)  | Have flow diagram that represnets registration system and the user list done  | 55 min  |  April 18th |   B  |
|  14 |  Work on the user list UI and list information (Development) | Redo initial UI for the user list webpage and add city information to the user informations displayed in the list  |  40 min | April 19th  |   C  |
|   15| Create the second version of the system diagram (Design)  |  Create a more accurate version of a system diagram | 20 min  | April 19th  | B |
| 16  |  Create a questionaire upload client questionaires in the appendix section (Evaluation) |  Have two client questionaires uploaded to the appendix | 25 min  | April 20th  |  D  |
| 17  | Add a base template options menu to all the pages (Development) | Have an options menu containg logout, user list, read articles...  | 30 min  |April 21st   |C     |
|  18 | Create a UML diagram for the web aplication (Design) | Have a Uml Diagram fimished for the SNS  | 15 min  | April 21st  |  B   |
| 19  | Update the test plan and add 2nd integration test, testing user list feature of the website (Testing)  | Have a written test about user list feature  |  10 min | April 22nd  |  B   |
|20   | Test accesing the user list from the main menu page (Testing) | Update the test plan with integration test relating allowing registered user to acces the table containing users of citio| 15 min  |  April 22 | B    |
|  21 | Test accesing a specific user from the user list feature. (Testing) | Update the test plan with integration test relating the feature that check a specific account from the user list  |  15 min | April 22nd  |  B   |
|  22 |  Creating new UI for the register, login, and home page of the website (Development) | Have more modern UI for the mentioned pages   | 40 min  | April 24th  |   C  |
|   23| Add a filter by city option for the user table (Development) |  Have a functioning feature to select the city of interest and see only relevant content creators | 20 min |  April 24th |  C   |
|   24| Add a search bar option for the user table (Development) | Have a functioning username search abr that will allow searching for a desried user/s fromthe user table  | 40 min  | April 24th  |  C   |
|   25| Do integration testing on the newly added filter options and the user list display option (Testing)  | See if all filter options work properly  | 10 min  | April 24th  |  B   |
|   26| Add a access token to the website (Development) |  Secure that users can not access the website options unless they are logged in | 35 min  |April 25th |C  |     
|   27|  Crate a feature to allow users to explore and learn about cities provided in Citio application (Development) | Have an option to learn about cities offered in Citio by clicking at the picture of them  | 1h 45 min | April 26th  |  C  |
|   28|  Create a flow diagram for the the user profile page  (Design) |Visually present the feature of viewing a specific profile thrrough a flow diagram   | 45 min  | April 26th  |   B  |
|  29 |  Write down the development process of fullfilling the success criteria 1 (login/register)(Development) |  Show the development process and computetional thinking behind the login / register options | 40 min  | April 26th  |  C   |
|  30 | Create a final version of the ER diagram that incldues new city informations in the database (Design) |  A new ER diagram shows most recent databse structure adequatelly |  10 min | April 26th  |   B  |
|  31 | Create a city database (Development)  | Have a database that conntains names, pcitures, desctiptions, fun facts. about cities from Citio  |  25min | April 26th  |   C  |
|  32 | Run code review testing for potential loops and loop nesting and see if any complex algorithms used need a comment to explain them to potential co-developers (Testing) | Have a more efficient code of higher quality and better coding practices that would make future co-development easier  | 25 min   | April 26th  |  B   |
| 33|Add a delete account option to the Social network website (Development) | Be able to delete your account | 15 min| April 28th|C |
|34|Write down a development process for fulfilling success criteria 2 (Posting reviews) (Development) | Show the developing process of the python code that fulfilled the 2nd success criteria stated in the success criteria stated above| 30 min |28th April |C |
|35 | write down development process for criteria 3,4,5 & 6 as well as the devlopment of the session tokens for the Citio website (Development) |Have a development process that is understandable and refers to computational thinking and shows the thinking process of developed algorithms| 1h 30 min|April 28th |C | 
| 36| Record the video showcasing how the website functions (Implementation) | Record a 4 minute video that shows all the features of the website and how client's criteria was met| 30 min| April 29th | D |
| 37 |Create a table of evaluation where success criteria was analyzed and explained how they were met  (Evaluation) | Have a table of evaluation where the processing of acomplishing criteria stated by the client was clearly explained and indicated| 40 min|April 29th | E|
|38 | Add user recommendation/ evaluation interview to shows how satisfied they are with the way criteria was answered and possible improvements that were sugegsted by the users to improve the social network (Test/Implement) | Have a interview which shows ideas for improving the application in the future| 10 min|April 30th | E|
|39| Redo wireframe diargam  (Design) | Wireframe Diargam is more undrstandable now|35 min |May 2nd | B |

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
12. Using Flask library in Python
## Sources
1. “Beautiful CSS Buttons Examples - CSS Scan.” 92 Beautiful CSS Buttons Examples - CSS Scan, https://getcssscan.com/css-buttons-examples. 
2. “Flask HTTP Methods, Handle GET &amp; Post Requests.” GeeksforGeeks, GeeksforGeeks, 2 Feb. 2023, https://www.geeksforgeeks.org/flask-http-methods-handle-get-post-requests/. 
3. “Cirrus CSS.” Cirrus, https://www.cirrus-ui.com/buttons/basics. 
4. Auth0. “JSON Web Tokens.” Auth0 Docs, https://auth0.com/docs/secure/tokens/json-web-tokens. 
5. “How to - Search Bar.” How To Create a Search Bar, https://www.w3schools.com/howto/howto_css_searchbar.asp. 

## Development

## Design aspect of the social network 
```.html

<style>
    .navbar { <!-- shape of the navigation bar and the circular shape -->
        overflow: hidden;
        background-color: #79bcff;   
        border-radius: 30px 30px 30px 30px;
        margin-bottom: 20px;
    }

    .navbar a { <!-- Shows the shape of a button/feature within the navigation bar, and it bolds the option where mousepad is currently on -->
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
</style>
```
Fig.10 Navigation Bar design style 

Fig.10 Shows the style features for the naigation bar used in the base template design of social network. The idea for a base template came from the patern recognition of the similar goals for final designs of differnet features throughout the social network. Instead of rewriting the template every time, I create a base template used for colors of all pages in social network website. In terms of web design, using a light blue color scheme can help create a sense of tranquility and trustworthiness, making it a good choice for websites related to health, finance, or technology. [^10]



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
Fig.11 HTML aspect of navigation bar using jinja template

Fig.11 Another patern that I have recognized was that I needed certain features one click away, regardless of what webpage of the website I was on. This is why I created a navigation bar that is located within the base template, allowing access to certain featrures from whicever page user is currently on. The technique that I used was manipulating Jinja templates in html, which allowed me to use loops and other python features within the html code. This allowed me to allow user to get redirected to another page through a hyper link using get_url function (Fig. 12)

## Success Criteria 1: The social network website will provide a  secure login and registration system. 
### Password encryption
```.py
from passlib.context import CryptContext

pwd_config = CryptContext(schemes = ["pbkdf2_sha256"],
                          default = "pbkdf2_sha256",
                          pbkdf2_sha256__default_rounds = 30000
                          )
```
Fig.12 Shows the encryption function used for securing users' data

Fig. 12 shows the process and encryption method used for the password hashing for the Social network website. To prevent any serious harm in the case of data leaking, where if the same password is used in multiple places, intruder can use that and the email for other web services, hurting the user in the process.
```.py
# this function receives unsafe password and returns the hashed password
def encrypt_password(user_passowrd):
    return pwd_config.encrypt(user_passowrd)

```
Fig. 13 shows method which calls the previously mentioned process of encryption.
In order to fulfill client's request for the website, safe and secure data storing is neccesary and it allows privacy of the user to stay at a desired level.

### Regsitration System
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
Fig. 14 shows the registration function for the social network website Citio. 

in Fig.14 The function takes the usernamme,city,email and a password which is then encrypted before storing everything into user database. we see that after running the query and successfully storing the infromation of the newly registered user, a user is redirected to the login page where it can access the website using credentials of the newly registered account.
When developing this part of code using generalisation I was able to recognize a way to solve one of the criteria requirements by including a option bar in the registration where a user would input the city  which he would write about. This helped with solving the problem of seeing irellevent content creators that are not located in my city.

### Login System
```.py
 if request.method == 'POST':
        email = request.form['email']
        passwd = request.form['passwd']
        db = database_worker("social_net.db")
        user = db.search(f"SELECT * from users where email ='{email}'
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
Fig.15 shows Login system feature of the website

Fig. 15 we see the login function of the social network website. After getting the credentials that a user inpted I developed an algorithm that searches through the suer database, looking for an account with a matching email address. Policy for the email address is to have symbol "@" and characters before and after it. If there is such a user, algorithm would then check if the encryption of the password they inputed matches the one in the database that was stored upon registration of the account. If it does, login is successful and a user is given a session token that lasts 30 minutes after which they would need to login again. 
With this said, this feature was successfully developed and client's criteria 1 was successfully met.

```.py
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

```
FIg.16 shows the JWT session token feature of the website. 

In Fig.16 shows the function used for the creation of the sesssion tokens. This important implementation was inspired by using computational thinking and decomposing the problem of webiste's safety. Even after implemtning cookies, one could still redirect to a page without signing in beforehand. This is why I generalized the algorithm for creating JWT session tokens [^11] which in turn allowed me to set a requirement that a user is logged in before accessing any features of the website. This improved security of the website and solved the previously decomposed problem of safety that the website had.

In order to successfully develop this I needed to have following things in my algorithm: The wraps function from functools module is used to preserve the original function's metadata (data contaitng information about certain data, in this case about the function). After that the decorated function checks if a token is present in the user's session. If a token is present, the function attempts to decode it using the 'jwt.decode' function. If the token is invalid, the user is redirected to the login page. If the token is valid, the decorated function is called with the original arguments and keyword arguments using the 'f' function. For this, args is used to pass a variable number of non-keyword arguments to the decorated function and kwargs is used to pass a variable number of keyword arguments to the decorated function. 



![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/criteria1proofPR4.gif)
Fig. 17 showcases the proof of criteria 4 being fulfilled, and visually represents the code and developing analyzed above.

## Success Criteria 2: The social network website will allow users to post reviews of the local places, containing title, date, and content. 
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
Fig. 18 shows the code developed in order to allow posting reviews on the social media website. The algorithm I developed uses if statements to gather article's title,content,time of posting, and checks if the information is being provided by the user currently sigend in. If that is the case a new post will be inserted and the page will be refreshed, now showing the newly posted article. I developed this algorithm using patern recognition from the login page where a similar type was used where after a certain validation a query was used which inserted data inputed into the database.
With this said, this feature ws successfully developed and client's criteria 2 was successfully met.

![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/criteria2proofPR4.gif)
Fig. 19 showcases the proof of criteria 4 being fulfilled, and visually represents the code and developing analyzed above.

## Success Criteria 3: The social network website will have a feature to display all users, their contact email, and the show the city about which they post. 
```.py
@app.route('/users')
@token_required
```
```.py
def users():
    # Checks if the user is authenticated by checking if the user.id cookie exists
    if request.cookies.get('user.id'):
        db = database_worker("social_net.db") # Creates a database worker object to perform SQL queries on the "social_net.db" database
        all_users = db.search("SELECT * FROM users")# Selects all users from the "users" table # selects username email adress and the city of the user
        db.close()# Closes the database connection
        
```
Fig. 20 shows the function used to showcase the list of all Citio users. It uses an algorithm that checks if the user has a valid cookie and then it shows the list of users extracted from the user database. Table is formated in the order: username, email, and city which is exactly what the criteria 3 required. The development stage was done by using the abstraction and not focusing on other relevant criteria yet (criteria 4 which is also about the user list display), until this one was solved.
With that, success criteria 3 was met, and a website now had a feature of showcasing its users.
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/criteria3proofPR4.gif)
Fig. 21 showcases the proof of criteria 4 being fulfilled, and visually represents the code and developing analyzed above.

## Success Criteria 4: The social network website will have an option to choose a specific city which you are interested in through a filter or use a username search filter, and see only relevant content creators. 
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
Fig. 22 shows the part of the code responsible for filter functions. User is able to filter the user list by 1) thier username and by 2) their city. Username search was done by creating algorithm that uses the search query inputed in the search bar by the user. Then I abstracted another problem that emerged when decompsing the searchf filter one, and that was it being case sensititve. I solved this by implementing .lower() function into existing algorithm. The city filter was done by using patern recognitionand generalizing the solution for adding cities from the search bar but instead of adding it to the database through the query, I searched users with the chosen city inside of that same database.
With this two filter options successfully presented, I have managed to met client's 4th success criteria.


![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/criteria4proofPR4.gif)
Fig. 23 showcases the proof of criteria 5 being fulfilled, and visually represents the code and developing analyzed above.


## Success Criteria 5: The social network website will to have a feature to see all reviews posted by a specific user, by selecting their profile. 
```.py
      users, posts = None, None
        user = db.search(f"SELECT * from users where id={user_id}")
        if user:
            posts = db.search(f"select * from posts where user_id={user_id}")
            user = user[0]  # remember search returns a list (should be one user so...

        return render_template("profile.html", user = user, posts = posts, current_user_id=int(current_user_id))
```
Fig. 24 shows the part of the code that is responsible for the option to go to a specific user's profile by clicking on their nickname. The procedure first decomposes the problem to quering users with an id is equal to that of the user that you clicked on. That should be only one user, and then another query inside of this algorithm will get all the posts created by this user which would be returned to the page whose template is being rendered, and we will be able to see them on his profile page. 
This Algorithm, after some modifications, successfully managed to meet eclient's criteria 5.

![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/criteria5proofPR4.gif)
Fig. 25 showcases the proof of criteria 5 being fulfilled, and visually represents the code and developing analyzed above.
## Success Criteria 6: The social network website will have an interactive option display available cities which user could explore, with an option to learn about each one, by simply clicking at the picture of it. 
```.py
@app.route('/cities', methods=["GET", "POST"])
@token_required
def cities():
    db = database_worker("social_net.db")
    all_cities = db.search("select * from cities")
    return render_template("cities.html", cities=all_cities)

```
cities.html
```.py
<body>
 <div class="picture-container">
    <img src="/static/CitioLogo.png" alt="logo">
  </div>
  <div class="header">
    Our Cities
  </div>

  <!-- Image containers -->
  <div class="image-container">
    {% for c in cities %}
      <div>
        <a href="{{ url_for('get_city', city_name=c[0]) }}">
          <img src="{{ c[1] }}" alt="">
        </a>
        <p>{{ c[2] }}</p>
      </div>
    {% endfor %}
  </div>

</body>
```
Fig. 26 shows the function that is used to render the template which will, using the base template (Fig.10), show the currently available cities in the Citio social network, and showing a picture their name and a small desription of the place. (These atributes can be seen in the city database Fig.7) The template that is rendered in this function has a feature that will send the user to a specific city page, when a picture of one of these cities ic clicked.

```.py
@app.route("/city/<city_name>")
def get_city(city_name):
    db = database_worker("social_net.db")
    city_data = db.search(f"select * from cities where name='{city_name}'")
    return render_template("city.html", city=city_data[0])

```
city.html
```
<body>

  <div class="header">
    {{ city[0] }}
  </div>

  <!-- Image container -->
  <div class="image-container">
    <img src="{{ city[1] }}" alt="Tokyo">
  </div>

  <!-- Content -->
  <div class="content">
<p>{{ city[4] }}</p>
  </div>

  <!-- Fun fact -->
  <div class="fun-fact">
    <p>{{ city[3] }}</p>
  </div>
</body>
```
Fig. 27 shows the function responsible for rendering the template of the webpage of the specific city chosen by the user in cities webpage that I refered to earlier (Fig. 21). In order to develop this specific city webpage, I went through a serious reasearch process on how to itterate my repetitive algorithm which repeated the same process 6 times, using 6 different html pages (one for each city). Recognizng this patern I was able to iterate a for loop using jinja in html and successfully meet client's 6th and final success criteria.

![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/criteria6proofPR4.gif)
Fig.28 showcases the proof of criteria 6 being fulfilled, and reflects on the code and developing analyzed above.

# Criteria D: Functionality
## Video showcase
## https://drive.google.com/file/d/1X0ebjV_iJ6acORMNIJx5kQhc6AHnULCD/view?usp=sharing

# Criteria E: Evaluation
## Evaluation table
|Criteria number| Criteria| Final product| Criteria success|
|---------------|----------|-------------------------------|--------------|
|1|The social network website will provide a secure login and registration system.|As it can be seen in Fig 17 I have met client's criteria with this login and registartion feature. This was seen in the user interview Fig 28| Succeeded|
|2|The social network website will allow users to post reviews of the local places, containing title, date, and content. |As it can be seen in Fig 19 I have met client's criteria with this login and registartion feature. This was seen in the user interview Fig 29|Succeeded|
|3|The social network website will have a feature to display all users, their contact email, and the city about which they post.|As it can be seen in Fig. 21 I have met client's criteria with this user list feature that shows all users and their contact email and city. This was seen in the user interview Fig. 29|Succeeded|
|4|The social network website will have an option to choose a specific city which you are interested in through a filter or use a username search filter, and see only relevant content creators.|As it can be seen in Fig. 23 I have met client's criteria with this interactive city feature. This was seen in the user interview Fig. 29|Succeeded|
|5|The social network website will to have a feature to see all reviews posted by a specific user, by selecting their profile.| As it can be seen in Fig. 25 I have met client's criteria with this feature that allowed to select a certain profile and looking at their reviews. This was seen in the user interview Fig 29|Succeeded|
|6|The social network website will have an interactive option display available cities which user could explore, with an option to learn about each one, by simply clicking at the picture of it.|As it can be seen in Fig 28 I have met client's criteria with this interactive feature to learn about cities offered in Citio. This was seen in the user interview Fig 29|Succeeded|


### All the evaluations of success from this tbale were gathered from the client interview (Fig. 29) in which interviewer (Citio representative) went through how satsified the user was with how success criteria was answered. Aditional data and research was gathered from the questionares where user's prefernces werer tested. This market testing can be seen in the [appendix](#Filled-out-questionaire-Tester-1)


Table 3 shows evaluation of all success criteria and the process to meeting them. It refers to the interview of a user of Citio who stated his opinnion on the quality of the webite through the criteria, and posible imporvements for the future.

## Client interview
This interview was conducted with one of Citio's users who evaluated if the criteria was met successfully and stated posible improvements to the application in the future.
## https://drive.google.com/file/d/10svpYaMdNyBv4XfzsgFjQ015OGXBtqFd/view?usp=sharing

Fig. 29 is a link to an interview with a Citio user. For the privacy reasons user stayed annonymous. The interview backed the succes of achiving all criteria and also gave some feedback for the future developing of the social network website.

## Reflection on the interview
After conductiong this interview

## Recommendation
After conducting the interview with the Citio user (Fig.29), user identified and justified two possible improvements for the future:

### 1. A system of liking and commenting on the posts:
This is something that we will deffinatelly consider for the future, as even though we aim to equally promote all posts and reviews, some are certainly better than others, and after reaching out to some other users, we discovered that they share the same opinion. we will stil make sue that this does not hurt our ideology of giving exposure to local shops withoiut a marketing team behind them, and only comments that are truly liked by the community will gain exposure. With this said, this suggestion will be the next step in the future phases of development.

### 2. More cities available in Citio application:
The thing that the user from the interview (FIg.29) mentioned multiple times was that even though all the cities relevant to him are on the website, as of this moment, he still thinks more cities are neccessary and that this is the final step to bring Citio to the next level and to gain deserved recognition. His friend s living outside this region can not really use the website even though they wanted to when he shared it with them. This is because right now our social media website mostly focuses on a very small region of Japan, and two biggest cities outside of that region. If there is no increase in the number of cities, website's popularity willnot inrease and further progress will not be possible. With that said, this is not a difficult addition and we will be developing this for sure.



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
[^11]: 4. Auth0. “JSON Web Tokens.” Auth0 Docs, https://auth0.com/docs/secure/tokens/json-web-tokens. 
