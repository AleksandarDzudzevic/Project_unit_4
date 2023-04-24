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
Being in love with exploring small local shops and restaurants, visiting tourist attractions, and everything else that a city has to offer, I have always faced the big challenge of finding them, as they can be hardly found on google maps where only a few gain exposure, eliminating smaller local shops and restaurants due to their lack of marketing. Another big problem is not having a place where my friends could see only the recipes I make, so that they could enjoy my exceptional cullinary skills. Current social networks gave these smaller businesses more exposure, but a user has to put great effort to narrow the search only to relevant local places located in their city. If an adequate solution is not presented soon, these smaller businesses will close due to a lack of traffic, resulting in market concentration, which in turn would hurt the economy and tourism of cities. This problem definition was established with the help of the data gathered through questionnaires.(referred to in the appendix)

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
1. The social network website will provide a login and registration system. 
[ Another big problem is not having a place where my friends could see only the recipes I make]
2. The social network website will allow users to post or delete their reviews of the local places, containing title, date, and content. [I have always faced the big challenge of finding them, as they can be hardly found on google maps where only a few gain exposure]
3. The social network website will have a feature to display all users and the city about which they post. [user has to put great effort to narrow the search only to relevant local places located in their city]
4. The social network website will have an option to choose a city which you are interested in, and see only relevant reviews. [user has to put great effort to narrow the search only to relevant local places located in their city]
5. The social network website will to have a feature to see all reviews posted by a specific user, by selecting their profile. [where only a few gain exposure, eliminating smaller local shops and restaurants due to their lack of marketing]
6. The social network website will have an interactive option display showing cities which user could explore, with an option to leran bout each one, by simply clicking at the picture of it. [these smaller businesses will close due to a lack of traffic]

# Criteria B: Design
## System Diagram
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/SystemDiagramPr2_v2.png)
Fig.3 shows the system diagram of the social network website
## Wireframe Diagram
## ER Diagram
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/project_4_er_diagram.png)
Fig.4 shows database structure of the social network website
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/user%20databse.png)
Fig.5 shows user database of the social network website, presented in the ER diagram (data provided in the example is not actual data gathered from any of the users.)
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/post%20database.png)
Fig.6 shows post database of social network website, presented in the ER diagram (data provided in the example is not actual data gathered from any of the users.)
## UML Diagram
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/Screenshot%202023-04-21%20at%2023.48.39.png)
Fig. 7 shows the class used for manipulating database, used for the website application 
## Flow Diagram
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/project4_flowch1_register.png)
Fig.8 Shows the flow diagram for the registration system of the Citio social network website
## Test plan
|Test Number|Description|Test Type| Target|Procedure|Expected Outcome|
|-----------|-----------|--------|-----------|-----------------|----|
|1|Account registration system|Unit testing|Have a fully functional registration system that checks if the proper values are inputed in the email and password fields|(1) Run Project_4.py (2) Click the register button on the login screen (3) Input data on all the fields (4) After filling in all the fields create an account (5) Try to login with the new account too see if it exists now| After following the procedure, a user should be able to login using the credentials of the newly created account|
|2|User list inspecting |Unit testing| be able to access the user list and see all the registered users and their username and the city which they post about.|(1)Run Project_4.py(2)Login using adequate credentials. (3)Choose the "see all users" option from the navigation bar.(4)Check if the redirected page shows a table containing: id,username, and city for each user| User is able to access the user list from the main menu and will be able to see all the citio users| 
|3|Accesing a specific user's post from the user list|Integration testing| Access a specific post uploaded by a user chosen from the user list|(1)Run Project_4.py(2)Login using adequate credentials. (3)Choose the "see all users" option from the navigation bar. (4) Choose a desired user and click on its nickname to get redirected to his profile. (5)Click on one of his posts and see if you are successfully redirected to a page to read it.| A user can choose read a specific post from a creator that he is interested |
|4|Uploading a post after logging in |Integration testing| | | |
|5|Code practices around html and css |Code Review| | | | 
|6| Commenting on complexed code practices |Code Review| | | |

## Record of Tasks
| Task No | Planned Action                                                | Planned Outcome                                                                                                 | Time estimate | Target completion date | Criterion |
|---------|---------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| 1       | Write the Problem Definition| Write a precise problem definition that identifies a problem, consequences of it, and a clear solution that is being proposed    | 25min         | April 7th    | A         |
| 2  |  Write down design statement | Have a first version of the design statement done  |  10 min | April 9th  |  A   |
| 3  |  Write down first success criteria established during the first user meeting | Have a first version of success criteria inspired by potential future users. Their opinions and preferences were gathered through a questionire  | 40min  | April 10th  |  A   |
|4| Write a proposed solution| Propose a solution for the Web application| 15 min| April 11th| A |
| 5 | Write down rationale for the proposed solution |  Have the firt version of rationale written down  | 45 min  | April 13th  |  A   |
| 6 | Rewrite success criteria initially stated | Have a clearer version of success criteria| 15 min  |  April 13th  | A|
| 7  | Add table of content  |  Add table of content at the top of the file |20 min| April 15th   |   A  |
|  8 | Create an ER diagram  |  Have an database structure representation for the social network website | 25 min  |  April 15th |   B  |
| 9 |  Create first version of SNS user interface welcome screen | Have user interface for the starting screen using CSS and HTML style features  |50 min  |  April 15th |  C   |
|  10| Create System diagram for SNS | Have a first version of system diagram done and ready to be presented to the client | 30 min  | April 16th  | B |
| 11|   Create functional registration system and have a first version UI for it  created |  Have a functional registration system for the SNS | 35 min    | April 17th    |C
|  12 | Create a active password policy check for the login feature  | Have a visual presentation showing if the password policy has been met or not  | 25 min | April 18th    | C
|  13 | Work on flow diargam for the registration system of the SNS  | Have flow diagram that represnets registration system done  | 35 min  |  April 18th |   B  |
|  14 |  Work on the user list UI and list information | Redo initial UI for the user list webpage and add city information to the user informations displayed in the list  |  40 min | April 19th  |   C  |
|   15| Create the second version of the system diagram  |  Create a more accurate version of a system diagram | 20 min  | April 19th  | B |
| 16  |  Create a questionaire upload client questionaires in the appendix section |  Have two client questionaires uploaded to the appendix | 25 min  | April 20th  |  D  |
| 17  | Add a base template options menu to all the pages  | Have an options menu containg logout, user list, read articles...  | 30 min  |April 21st   |C     |
|  18 | Create a UML diagram for the web aplication  | Have a Uml Diagram fimished for the SNS  | 15 min  | April 21st  |  B   |
| 19  | Update the test plan and add 2nd integration test, testing user list feature of the website  | Have a written test about user list feature  |  10 min | April 22nd  |  B   |
|20   | Test accesing the user list from the main menu page  | Allow registered user to acces the table containing users of citio| 15 min  |  April 22 | B    |
|  21 | Test Accesing a specific user from the user list feature.  | Update the test plan with integration test relating the feature that check a specific account from the user list  |  15 min | April 22nd  |  B   |
|  22 |  Crreating new UI for the register, login, and home page of the website | Have more modern UI for the mentioned pages   | 40 min  | April 24th  |   C  |
|   23|   |   |   |   |     |
|   24|   |   |   |   |     |
|   25|   |   |   |   |     |
|   26|   |   |   |   |     |
|   27|   |   |   |   |     |
|   28|   |   |   |   |     |
|  29 |   |   |   |   |     |
|  30 |   |   |   |   |     |
|  31 |   |   |   |   |     |
|  32 |   |   |   |   |     |

# Criteria C: Development
## Tools and techniques used
No definition!  
## Sources

## Development
Explain how I was challenged and how I solved with explaining the lines of codes.

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

