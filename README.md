# Citio social network
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/dalee_unit4_project.png)
Fig.1 shows the picture created for Citio using DALL-E 2 [^1]
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
Being in love with exploring small local shops and restaurants, visiting tourist atractions and everything else that a city has to offer, I have always faced a big challenge of finding them, as they can be hardly found on google maps where only few gain exposure, eliminating smaller local shops and restaurants due to their lack of marketing. Current social network gave these smaller businesses more exposure, but a user has to put great effort to narrow the search only to relevant local places located in their city. If an adequate solution is not presented soon, these smaller businesses will close due to lack of trafic, resulting in market concentration, which in turn would hurt economy and tourism of cities. 

## Design Statement
To tackle this issue I will design a new creative social network that would allow people located in the same city to connect with others through sharing interesting local places, culinary expiriences, astonsihing nature and everything one city has to offer. The development will be done using the software Flask framework in Python, CSS and HTML. It will take around 5 weeks to develop and will be evaluated according to the success criteria stated below by the client.

## Rationale for Proposed Solution


### Why Python?
Python contains many versatile features, which make it a better choice compared to other languages, for example PHP[^2]. Python's Flask framework is ideal for developing social network websites due to its lightweight and flexible nature [^3]. Flask's simplicity and ease of use make it an excellent choice for this project, allowing developers to focus on the website's core features and functionality. It also offers a range of libraries and extensions, making it easier to implement complex features such as authentication and database connectivity, when compared to its competitors such as PHP or ruby [^4]. With Python's object-oriented programming, developers can write code that is easy to read, modify, and maintain, which is essential when creating a complex web application such as a social network website. Additionally, Python has an active community of developers who offer support and resources, making it easier to learn and develop with the language.

### Why SQL
To store the vast amounts of data needed for a social network website, a reliable and efficient database is essential. While non-SQL databases can be an option, SQL databases offer several advantages that make them better suited for this purpose. The main advantage of SQL databases is their ability to handle large amounts of data efficiently, thanks to their relational structure[^5]. The relational structure of SQL databases makes it easier to manage and query data, as it is stored in tables. This feature also ensures that data is consistent and accurate, as it is subject to strong data integrity constraints[^6]. With all the data that is being stored for this social network website, an SQL database is essential to ensure efficient data handling and management.

### Why HTML
HTML is the standard markup language used to create web pages and it provides the structure and content of a website[^7]. Compared to other alternatives such as Flash, HTML is more widely supported, making it a better choice for cross-platform compatibility[^8]. Additionally, HTML is more search engine friendly than other technologies such as JavaScript, which can lead to better search engine rankings[^9].


## Success Criteria
1. The social network website will provide a login and registration system.
2. The social network website will allow users to post their reviews of the local places, containing title, date, and content.
3. The social network website will have a feature to display all users and the city about which they post.
4. The social network website will have an option to choose a city which you are interested in, and see only relevant reviews.
5. The social media will allow a user signed in to upload and delete posts from their account.
6. The social network website will to have a feature to see all reviews posted by a specific user, by selecting their profile.

# Criteria B: Design
## System Diagram
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/Project4systemdiagram.png)
Fig.3 shows the system diagram of the social network website
## Wireframe Diagram
## Flow Diagram
## ER Diagram
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/project_4_er_diagram.png)
Fig.4 shows database structure of the social network website
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/user%20databse.png)
Fig.5 shows user database of the social network website, presented in the ER diagram (data provided in the example is not actual data gathered from any of the users.)
![](https://github.com/AleksandarDzudzevic/Project_unit_4/blob/main/post%20database.png)
Fig.6 shows post database of social network website, presented in the ER diagram (data provided in the example is not actual data gathered from any of the users.)
## UML Diagram
## Flow Diagram
## Test plan
|Test Number|Description|Test Type| Target|Procedure|Expected Outcome|
|-----------|-----------|--------|-----------|-----------------|----|
|1|Account registration system|Unit testing|Have a fully functional registration system that checks if the proper values are inputed in the email and password fields|(1) Run Project_4.py (2) Click the register button on the login screen (3) Input data on all the fields (4) After filling in all the fields create an account (5) Try to login with the new account too see if it exists now| After following the procedure, a user should be able to login using the credentials of the newly created account|
|2| |Unit testing| | | | 
|3| |Integration testing| | | |
|4| |Integration testing| | | |
|5| |Code Review| | | | 
|6| |Code Review| | | |

## Record of Tasks
| Task No | Planned Action                                                | Planned Outcome                                                                                                 | Time estimate | Target completion date | Criterion |
|---------|---------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| 1       | Write the Problem Definition| Write a precise problem definition that identifies a problem, consequences of it, and a clear solution that is being proposed    | 25min         | April 7th    | A         |
| 2  |  Write down design statement | Have a first version of the design statement done  |  10 min | April 9th  |  A   |
| 3  |  Write down first success criteria established during the first user meeting | Have a first version of success criteria inspired by potential future users. Their opinions and preferences were gathered through a questionire  | 40min  | April 10th  |  A   |
| 4  | Write down rationale for the proposed solution |  Have the firt version of rationale written down  | 45 min  | April 13th  |  A   |
| 5 | Rewrite success criteria initially stated | Have a clearer version of success criteria| 15 min  |  April 13th  | A|
| 6  | Add table of content  |  Add table of content at the top of the file |20 min| April 15th   |   A  |
|  7 | Create an ER diagram  |  Have an database structure representation for the social network website | 25 min  |  April 15th |   B  |
| 8  |  Create first version of SNS user interface welcome screen | Have user interface for the starting screen using CSS and HTML style features  |50 min  |  April 15th |  C   |
|  9| Create System diagram for SNS | Have a first version of system diagram done and ready to be presented to the client | 30 min  | April 16th  | B |
| 10|   Create functional registration system and have a first version UI for it  created |  Have a functional registration system for the SNS | 35 min  |   | April 17th    |C
|  11 |   |   |   |   |     |
|  12 |   |   |   |   |     |
|  13 |   |   |   |   |     |
|   14|   |   |   |   |     |
| 15  |   |   |   |   |     |
| 16  |   |   |   |   |     |
|  17 |   |   |   |   |     |
| 18  |   |   |   |   |     |
|  19 |   |   |   |   |     |
|  20 |   |   |   |   |     |
|  21 |   |   |   |   |     |
|   22|   |   |   |   |     |
|  23 |   |   |   |   |     |
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

# Works cited
[^1]: Open AI DALL-E 2 (https://labs.openai.com/s/uCyXQVhhqoXmRdc2Y9KDUyIR)
[^2]: Sengar, Ritesh. “Python vs PHP: Which Is Better for Web Development?” Hackernoon, 7 Jan. 2021, hackernoon.com/python-vs-php-which-is-better-for-web-development-cj1236mj. 
[^3]: "Welcome to Flask." Flask Documentation, 15 Jan. 2023, flask.palletsprojects.com/en/2.1.x/. 
[^4]: Grinberg, Miguel. Flask Web Development: Developing Web Applications with Python. 2nd ed., O'Reilly Media, Inc., 2018. 
[^5]: “What Is a Database?” Oracle, https://www.oracle.com/database/what-is-database/. 
[^6]: "What is SQL?" W3Schools, W3Schools, https://www.w3schools.com/sql/
[^7]: "HTML Introduction." W3Schools, W3Schools, https://www.w3schools.com/html/html_intro.asp
[^8]: "Flash vs. HTML5." Digital.gov, 17 Dec. 2015, https://digital.gov/resources/flash-vs-html5/.
[^9]: "Why You Need an SEO-Friendly Website." SEO Werkz, 11 Jan. 2022, https://www.seowerkz.com/why-you-need-an-seo-friendly-website/.

