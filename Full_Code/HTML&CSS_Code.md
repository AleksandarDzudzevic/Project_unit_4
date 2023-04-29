# Html Code for the Citio webite

## Base template
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    {% if title %}
    <title>{{ title }}</title>
    {% else %}
    <title>Welcome to the most popular SNS</title>
    {% endif %}
    <link rel="stylesheet" href="/static/my_style.css">

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
</head>
<body>
<div class="navbar">
    <a href="{{ url_for('index') }}">Home</a>
    <a href="{{ url_for('users') }}">Users</a>
    <a href="{{ url_for('cities') }}">Cities</a>
    <a href="{{ url_for('posts') }}">Posts</a>
    <a href="{{ url_for('my_profile') }}">Your profile</a>
    <a href="{{ url_for('logout') }}">Logout</a>
    <a href="{{ url_for("delete_profile") }}">Delete the account</a>
</div>
{% block content %}

<div class="container">
    <div class="image">
        <img src="/static/dream_TradingCard.jpg" alt="citation_picture">
    </div>
    <div class="options">
        <a href="{{ url_for('users') }}">Show all users</a>
        <a href="{{ url_for('posts') }}">Show all posts</a>
        <a href="{{ url_for('cities') }}">Our Cities</a>
        <a href="{{ url_for('my_profile') }}">Your profile</a>
        <a href="{{ url_for('register') }}">Create Account</a>
    </div>
</div>
{% endblock %}
</body>
</html>

```
## Login code
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Welcome to the best SNS</title>
</head>

<link rel="stylesheet" href="/static/my_style.css">
<style>
   body{

 background-color: #b8d8ff; background-image: radial-gradient(circle at right top, rgb(255, 255, 255), rgba(0, 255, 255, 0)), radial-gradient(circle at left bottom, rgb(129, 184, 248), rgba(255, 20, 146, 0));
   }
  p{

  }
</style>
<body>
 <form method="post">
     <div class="picture-container">
         <img src="/static/CitioLogo.png" alt="logo">
</div>
     <h2>Login to Citio</h2>
     <div>
         <label for="">Email</label>
         <input type="email" name="email">
     </div>
        <div class="form__field">
            <input type="password"  name="passwd" class="form__input" pattern=".{6,}" required>
            <span class="icon"></span>
        </div>
     <div>
         <input type="submit" name="" value="Log In">
     </div>
    <div>
   <p style="color: #333; font-size: 18px;">Don't have an account yet?</p>
   <ol style="list-style-type: none; margin: 0; padding: 0;">
      <li><a href="{{ url_for('register') }}" style="color: #007bff; font-size: 22px; text-decoration: none;">Create an Account</a></li>
   </ol>
</div>

 </form>
</body>
</html>
```
## Regsitration Code
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Register - Citio</title>
    <style>
        body {
            background-color: #F6F7F9;
            font-family: Arial, sans-serif;
            font-size: 16px;
        }
        form {
            max-width: 500px;
            margin: 0 auto;
            background-color: #FFFFFF;
            border-radius: 10px;
            padding: 20px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }

        h2 {
            text-align: center;
            font-weight: bold;
            color: #79bcff;
            margin-bottom: 30px;
        }
        label, input, select {
            display: block;
            width: 100%;
            margin-bottom: 20px;
            color: #555555;
        }
        input[type="text"], input[type="email"], input[type="password"], select {
            border: none;
            border-radius: 5px;
            padding: 10px;
            font-size: 16px;
            background-color: #F6F7F9;
            box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.1);
        }
        input[type="text"]:focus, input[type="email"]:focus, input[type="password"]:focus, select:focus {
            outline: none;
            background-color: #FFFFFF;
            box-shadow: 0px 0px 5px rgb(121, 188, 255);
        }
        input[type="submit"] {
            background-color: #79bcff;
            color: #FFFFFF;
            border: none;
            border-radius: 5px;
            padding: 15px;
            font-size: 16px;
            cursor: pointer;
            transition: background-color 0.2s ease-in-out;
        }
        input[type="submit"]:hover {
            background-color: #429efc;
        }
        option {
            color: #555555;
        }
    </style>
</head>
<body>
    <form method="post">

     <div class="picture-container">
         <img src="/static/CitioLogo.png" alt="logo">
    </div>
        <h2>Create an Account</h2>
        <div>
            <label for="username">Username</label>
            <input type="text" id="username" name="username" required>
        </div>
        <div>
            <label for="email">Email</label>
            <input type="email" id="email" name="email" required>
        </div>
        <div>
            <label for="password">Password (at least 6 characters)</label>
            <input type="password" id="password" name="password" pattern=".{6,}" required>

        </div>
        <div>
            <label for="city">City</label>
            <select id="city" name="city" required>
                <option value="">--Please choose an option--</option>
                <option value="Karuizawa">Karuizawa</option>
                <option value="Saku">Saku</option>
                <option value="Nagano City">Nagano City</option>
                <option value="Ueda">Ueda</option>
                <option value="Tokyo">Tokyo</option>
                <option value="Osaka">Osaka</option>
            </select>
        </div>
        <div>
            <input type="submit" value="Register">
        </div>

<div style="text-align:center; margin-top:20px;">
    <a href="{{ url_for('login') }}">Create an Account</a>
</div>
    </form>
</body>
</html>
```
## Profile code
```
{% extends "base_template.html" %}
{% block content %}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    {% if user %}
    <title>{{ user[1]}}</title>
    {% else %}
    <title>User does not exist</title>
    {% endif %}
</head>
<link rel="stylesheet" href="/static/my_style.css">

<style>
     h1 {
            text-align: center;
            color: #ffffff;
            font-size: 50px;
            font-weight: bold;
            text-shadow: 2px 2px #17a3ec;
        }

        h2 {
            font-size: 40px;
            color: #ffffff;
            text-shadow: 1px 1px #000000;
        }
.post-form {
border: 1px solid #00074d;
border-radius: 5px;
padding: 20px;
margin: 20px 0;
background-color: #fff;
}

.post-form h2 {
font-size: 24px;
margin-bottom: 10px;
}

.post-form input[type="text"], .post-form textarea {
border: none;
border-bottom: 1px solid #00074d;
font-size: 18px;
padding: 5px;
margin-bottom: 10px;
width: 100%;
}

.post-form input[type="submit"] {
background-color: #00074d;
border: none;
border-radius: 5px;
color: #fff;
font-size: 18px;
padding: 10px;
cursor: pointer;
}
p{
    font-size: 35px;
}
a{

}
</style>
<body>
  <div class="picture-container">
         <img src="/static/CitioLogo.png" alt="logo">
    </div>
{% if user %}
    <h1>Welcome {{ user[4] }}</h1>
    {% if posts | length > 0 %}
    <p>{{ user[4] }}'s posts are:</p>
        <table>
            <tr>
                <td>id</td>
                <td>title</td>
                <td>Content</td>
                <td>date published</td>
            </tr>
            {# template language is jinja2 #}
            {% for p in posts %}
            <tr>
                <td>{{ p[0] }}</td>
                <td>{{ p[1].title() }}</td>
                <td>{{ p[2] }}</td>
                <td>{{ p[4] }}</td>
            </tr>
            {% endfor%}
        </table>
        {% else %}
        <p>You do not have any posts yet</p>
        {% endif %}
        <div class="post-form">
    {% if user %}
    {% if user[0] == current_user_id %}
        <h2>Create a new post</h2>
        <div class="post-form">
            <form method="post">
                <input type="text" name="title" placeholder="Title" maxlength="30">
                <textarea name="content" placeholder="Write your post here..." maxlength="150"></textarea>
                <input type="submit" value="Create a new post">
            </form>
        </div>
    {% endif %}
{% endif %}
{% else %}
    <h1>USER DOES NOT EXIST</h1>
{% endif %}
</body>
</html>
{% endblock %}
```
## Users list Code
```
{% extends "base_template.html" %}

{% block content %}
    <!DOCTYPE html>
    <html lang="en">
    <style>
        select {
            font-size: 17px;
            border-radius: 30px 30px 30px 30px;
            background-color: #F0FFFF;
            color: #000000;
            margin-right: 10px;
        }
        button, input[type="submit"] {
            font-size: 17px;
            border-radius: 30px 30px 30px 30px;
            background-color: #F0FFFF;
            color: #000000;
        }
        label{
            font-size:20px;
            font-style: italic;
        }
    </style>
    <h1>All Users</h1>
    <form method="GET" style="display: inline-block;">
        <label for="city">Filter by City:</label>
        <select name="city" id="city">
            <option value="">All Cities</option>
            <option value="Karuizawa">Karuizawa</option>
            <option value="Saku">Saku</option>
            <option value="Nagano City">Nagano City</option>
            <option value="Ueda">Ueda</option>
            <option value="Tokyo">Tokyo</option>
            <option value="Osaka">Osaka</option>
        </select>
        <button type="submit">Search</button>
    </form>
    <form method="GET" style="display: inline-block;">
        <label for="search_query">Search by username:</label>
        <input type="text" id="search_query" name="search_query">
        <button type="submit">Search</button>
    </form>
    <table>
        <thead>
            <tr>
                <th>ID</th>
                <th>Name</th>
                <th>City</th>
                <th>Email</th>
            </tr>
        </thead>
        <tbody>
            {% for user in users %}
                {% if not city or user[3] == city %}
                    {% if not search or search.lower() in user[4].lower() %}
                        <tr>
                            <td>{{ user[0] }}</td>
                            <td><a href="{{ url_for('profile',user_id=user[0]) }}">{{ user[4] }}</a></td>
                            <td>{{ user[3] }}</td>
                            <td>{{ user[1] }}</td>
                        </tr>
                    {% endif %}
                {% endif %}
            {% endfor %}
        </tbody>
    </table>
    </html>
{% endblock %}
```
## All cities page Code
```
{% extends "base_template.html" %}
{% block content %}
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Citio Cities</title>
  <meta charset="utf-8">
  <style>
      .header {
      text-align: center;
      font-size: 60px;
      margin-top: 45px;
      color: #ffffff;
      background-color: #79bcff;
    }

   /* Style the individual images */
.image-container img {
  width: 370px;
  height: 220px;
  border-radius: 30px;
  margin: 20px;
  border: 2px solid #ddd;
}

/* Add spacing between the images */
.image-container div {
  margin: 20px;
}

/* Center the images and text */
.image-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  margin-top: 50px;
}

.caption {
  text-align: center;
  font-size: 30px;
  margin-top: 20px;
  font-style: italic;
  color: #117bff;
}

p {
  font-size: 20px;
  color: #2d2b2b;
    font-style: italic;
}

  </style>
</head>
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
</html>
{% endblock %}
```
## Specific City Code
```
{% extends "base_template.html" %}
{% block content %}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>{{ city[0] }}</title>

  <style>
    /* Style the header */
    .header {
      text-align: center;
      font-size: 60px;
      margin-top: 45px;
      color: #ffffff;
      background-color: #79bcff;
    }

    /* Style the container for the image */
    .image-container {
      display: flex;
      justify-content: center;
      align-items: center;
      margin-top: 50px;
    }

    /* Style the image */
    .image-container img {
      width: 500px;
      height: 300px;
      border-radius: 30px 30px 30px 30px;
      border: 2px solid #ddd;
    }

    /* Style the content */
    .content {
      text-align: center;
      margin-top: 50px;
      margin-bottom: 50px;
      font-size: 25px;
    }

    /* Style the fun fact */
    .fun-fact {
      text-align: center;
      margin-top: 50px;
      margin-bottom: 50px;
      font-size: 20px;
      font-style: italic;
      color: #79bcff;
    }
  </style>
</head>
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
</html>
{% endblock %}

```
## Post list Code
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <div class="picture-container">
        <img src="/static/CitioLogo.png" alt="logo">
    </div>
    <title>Citio posts</title>
</head>
<link rel="stylesheet" href="/static/my_style.css">
<body>
{% extends "base_template.html" %}
{%  block content %}
<h1>All Posts</h1>
<table style="width: 100%; border-collapse: collapse;">
    <tr>
        <th style="border: 1px solid #ddd; padding: 8px; text-align: left;">id</th>
        <th style="border: 1px solid #ddd; padding: 8px; text-align: left;">title</th>
        <th style="border: 1px solid #ddd; padding: 8px; text-align: left; max-width: 200px; white-space: nowrap; overflow: hidden; text-overflow: ellipsis;">content</th>
        <th style="border: 1px solid #ddd; padding: 8px; text-align: left;">date published:</th>
    </tr>
    {% for u in posts %}
    <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: left;">{{ u[0] }}</td> {# id #}
        <td style="border: 1px solid #ddd; padding: 8px; text-align: left;;">{{ u[1] }}</td>
    <td style="border: 1px solid #ddd; padding: 8px; text-align: left; max-width: 200px; white-space: pre-wrap; overflow-wrap: break-word;">{{ u[2] }}</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: left;">{{ u[4] }}</td> {# city #}
    </tr>
    {% endfor %}
</table>
{% endblock %}
</body>
</html>

```
## Home Page Code
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Welcome to CITIO</title>
    <link rel="stylesheet" href="/static/my_style.css">
    <style>
        body {
            background-color: #F0FFFF;
        }
        .container {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            margin: 10px;
        }
        .options {
            list-style-type: none;
            margin: 100px;
            padding: 0;
        }
        .options li {
            margin-bottom: 10px;
        }
        .options li a {
            display: block;
            padding: 20px;
            background-color: #6495ED;
            color: #FFFFFF;
            font-size: 28px;
            border-radius: 10px;
            text-decoration: none;
        }
        .options li a:hover {
            background-color: #4169E1;
        }
        .picture {
            border-radius: 30px 30px 30px 30px;
            margin-right: 20px;
            overflow: hidden;
        }
        .picture img {
            display: block;
            width: 400px;
            height: 600px;
            object-fit: cover;
        }
    </style>
</head>
<body>

     <div class="picture-container">
         <img src="/static/CitioLogo.png" alt="logo">
</div>
    <h1>🏙️Welcome to Citio⛩️</h1>
    <div class="container">
        <div class="picture">
            <img src="/static/dream_TradingCard.jpg" alt="citation_picture">
        </div>
        <ul class="options">
            <li><a href="{{ url_for('users') }}">Show all users</a></li>
            <li><a href="{{ url_for('cities') }}">Our Cities</a></li>
            <li><a href="{{ url_for('posts') }}">Show all posts</a></li>
            <li><a href="{{ url_for("my_profile") }}">Your profile</a></li>
            <li><a href="{{ url_for('register') }}">Create Account</a></li>
            <li><a href="{{ url_for('logout') }}">Logout</a></li>
        </ul>
        <div class="picture">
            <img src="/static/dream_TradingCard2.jpg" alt="citation_picture">
        </div>
    </div>
</body>
</html>

```
## CSS Template Code
```
body{
 background-color: #b8d8ff; background-image: radial-gradient(circle at right top, rgb(255, 255, 255), rgba(0, 255, 255, 0)), radial-gradient(circle at left bottom, rgb(167, 207, 255), rgba(255, 20, 146, 0));
}
table{
    background-color: #b8d8ff;
}
h1{
    text-align: center;
    border-radius: 30px 30px 30px 30px;
    margin-top: 5px;
}
.container{
    display: block;
    margin:0 auto;
    background-color: #c0ddff;
    padding: 50px;
    border-radius: 30px 30px 30px 30px;

}
   img{
       border-radius: 30px 30px 30px 30px;
       position: center;
   }
    .picture-container {
    display: flex;
    justify-content: center;
    }

    .picture-container img {
    margin: 0 auto;
    display: block;
    }
    form{
        font-size: 35px;
        text-align: center;
        margin: 0 auto;
        width: 50%;
    }
    h2 {
        font-family: Arial, sans-serif;
        font-size: 2em;
        font-weight: bold;
        color: #ffffff;
        text-shadow: 2px 2px #5eb0d5;
        margin: 0 0 100px;
        border-radius: 30px 30px 30px 30px;
        padding: 8px;
        background-color: #9fcdff;
        border: 1px solid #ffffff;
        box-shadow: 2px 2px #050e65;
    }
    input[type="email"]{
        font-size: 20px;
        padding: 20px;
        border-radius: 8px;
        border: none;
        background-color: #f8f8f8;
        margin-bottom: 20px;
        width: 100%;
        box-sizing: border-box;
    }
    input[type="password"]{
        font-size: 20px;
        padding: 20px;
        border-radius: 8px;
        border: none;
        background-color: #ffffff;
        margin-bottom: 20px;
        width: 100%;
        box-sizing: border-box;
        outline: 0;
        }

.form__field {
  position: relative;
}

.form__field .icon {
  position: absolute;
  right: 1em;
  top: 50%;
  transform: translateY(-50%)
}

.form__input {
  border-radius: 0.25em;
  border-style: solid;
  border-width: 2px;
  font-size: 1.5rem;
  padding: 0.5em 4em 0.5em 2em;
}

.form__input:valid {
  border-color: forestgreen;
}

.form__input:valid + .icon::after {
  content: '😃';
}

.form__input:invalid {
  border-color: firebrick;
}

.form__input:invalid + .icon::after {
  content: '😳';
}


    input[type="submit"]{
        background-image: linear-gradient(#98c8ff, #ffffff);
        border: 0;
        border-radius: 4px;
        box-shadow: rgba(0, 0, 0, .3) 0 5px 15px;
        box-sizing: border-box;
        color: #000000;
        cursor: pointer;
        font-family: Montserrat,sans-serif;
        font-size: 20px;
        margin: 5px;
        padding: 5px 25px;
        text-align: center;
        user-select: none;
        -webkit-user-select: none;
        touch-action: manipulation;
    }
    p{
        color: #0d70ea;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-size: 25px;
        text-align: center;
    }
    ol{
         color: #5d5d5d;
        font-family: "Apple LiSung", serif;
        font-size: 25px;
        text-align: center;
    }


         body {
            background-color: #fff9ec;
        }
        h1 {
            text-align: center;
            background-color: #293cff;
            color: #fff;
            padding: 15px;
            font-size: 70px;
        }
        li {
            list-style: none;
            margin: 0;
            padding: 0;
            border-color: black;
            text-align: center;
            font-size: 20px;
        }
        li ol {
            margin-bottom: 10px;
        }
        li ol a {
            color: #1f8cff;
            text-decoration: none;
            text-align: center;
            font-size: 40px;
        }
        li ol a:hover {
            color: #fff;
            background-color: #00074d;
            padding: 5px;
            text-align: center;
            border-radius: 5px;
            text-size: 50px;
        }

h1 {
  font-family: Arial, sans-serif;
        font-size: 5em;
        font-weight: bold;
        color: #ffffff;
        text-shadow: 2px 2px #00074d;
        margin: 0 0 100px;
        padding: 5px;
        background-color: #a7d3fd;
        border: 1px solid #ffffff;
        border-radius: 5px;
        box-shadow: 2px 2px #050e65;
}
table {

  font-family: arial, sans-serif;

  border-collapse: collapse;

  width: 100%;

}


td, th {

  border: 1px solid #00074d;

  text-align: left;

  padding: 8px;

}


tr:nth-child(even) {

  background-color: #ffffff;

}
.menu-btn {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 30px;
  height: 22px;
  position: fixed;
  top: 20px;
  right: 20px;
  cursor: pointer;
  z-index: 9999;
}

.menu-btn span {
  width: 100%;
  height: 2px;
  background: #333;
  margin: 2px 0;
  transition: all 0.2s ease-in-out;
}

.menu-btn.open span:nth-child(1) {
  transform: translateY(6px) rotate(45deg);
}

.menu-btn.open span:nth-child(2) {
  opacity: 0;
}

.menu-btn.open span:nth-child(3) {
  transform: translateY(-6px) rotate(-45deg);
}

.menu {
  position: fixed;
  top: 0;
  right: 0;
  width: 0;
  height: 100vh;
  background: #FFF;
  z-index: 9998;
  overflow: hidden;
  transition: width 0.3s ease-in-out;
}

.menu.open {
  width: 200px;
}
.menu ol {
  margin: 0;
  padding: 0;
  list-style: none;
  text-align: right;
}
.menu ol li {
  padding: 10px 20px;
  border-bottom: 1px solid #EEE;
  font-size: 16px;
}

```
