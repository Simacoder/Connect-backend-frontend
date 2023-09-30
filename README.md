# Connect BackEnd to FrontEnd
The project to connect Back-End to Front-End using Django 

This is how to connect Django backend framework to React front library

We are goint to create simple data entry application in the backend and return data on the frontend from the backend using Axios library

Reason to choose React with Django:

Both React and Django are the most popular libraries and frameworks in their respective domains. React’s SPA optimization and Django’s powerful features make it even better. They have large community support and provide immediate assistance whenerver needed.

# APIs
-RestFramework 
-Cors-header

# Backend 

- 1- The Back-end where we're going to create API using DJANG-REST

- 2- and the front-end where we will interact directly with the API using React JS.

So, we're going to create a simple project to write employee's name and his department in the backend and then connect react as our main frontend to django server to fetch data and display it in our react application.

We will need django isntalled obviously,

and I will work in virtual environemnt, i will use pipenv, so if you dont'have it, you can pip install pipenv and once that finsihed

go ahead and pipenv install djangorestframework first which is a toolkit for building our API; and also we need to

pipenv isntall django-cors-headers for handling the server headers required for

Cross-Origin Resource Sharing (CORS) and this is to add CORS headers which allows our API to be accessed on other domains.

and later we will add corsheaders in INSTALLED_APP in settings file in django.

models.py: Now let’s create a database model for our project.

Here is models.py file of our app : ewmployee and department are two fields that are used to store the name of the empl and her or his department respectively.

serializer.py: Create serializer.py inside the app folder.

and Serializers are basically used to convert complex data to native Python datatypes that can then be easily rendered into JSON(Which we are going to use in React on the client side).

views.py: Here is views.py in which we can create our method like GET, PUT, POST, DELETE.

We will have only two methods, get and post

# Frontend

- npx create-react-app frontend

- then cd frontend npm install axios

- Axios is the main tool for connecting back-end with front-end. All the requests will be sent to the server (back-end) with the help of Axios.

- Inside App.js

import React from 'react';
class App extends React.Component {
render() {
return(

# AUTHOR
- Simanga Mchunu