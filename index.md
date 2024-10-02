---
layout: default
---

# Coding Workshop Guide

This guide is designed for you to follow along as we step through todays workshop. 

You have a hard copy where you can take notes. Code snippets are available via this webpage as we code along together.



# Welcome!

We’re thrilled to have you join this Coding Waves Workshop! 😊 In this tutorial, we’ll guide you through the fascinating world of web technologies, revealing the different components that come together to create a web application.

This journey may feel like an adventure into the unknown — but don’t worry! You’ve already taken the brave first step by being here, and we’re confident you will do great. 🌟


 - - - -

# Introduction

Have you ever felt like the world is becoming more tech-driven, but you're not quite there yet? Or maybe you've thought the world of software is just too complex to dive into on your own?

Well, we’ve got some great news for you! Programming isn’t as daunting as it seems, and we’re here to show you just how fun it can be.

This tutorial won’t instantly make you a programmer — but that’s okay! Becoming skilled in this field takes time, practice, and patience. What we aim to do is show you that programming and website creation aren’t as complicated as they might appear. We’ll break things down into manageable pieces so that you won’t feel overwhelmed.

We hope to spark a Love for Tech in you, just like it did for us!

 - - - -
 
## What you will learn from this workshop?

By the end of this workshop, you’ll have created a small, functional web application. Today we will learn how to fetch data from a server up in the cloud - how cool is that!?

![image](/assets/Slide11.png)

 - - - -

# Environment Setup

One of the first tools we will use is JSFiddle. JSFiddle is a popular, browser-based development sandbox environment where you can write, edit, and run code in HTML, CSS and Javascript. These code snippets allow us to see the results in real-time.

Try it out! Navigate to the JSFiddle Workspace by typing 
```
 https://jsfiddle.net/ 
```
in your browser.


When you open JSFiddle, you will notice the workspace is divided into four sections:
*  HTML Panel: This is where you’ll write the structure of your webpage.
*  CSS Panel: Use this panel to style your HTML elements.
*  JavaScript Panel: Here’s where the functionality of your web application comes to life.
*  Result Panel: This section displays the output of your code. It will update as you make changes.


 - - - -
 

# HTML 

HTML (HyperText Markup Language), is the foundation of every web page. It combines Hypertext (which connects different web pages) with Markup Language (which structures text within tags to form the building blocks of a webpage). For more information, see https://www.w3schools.com/html/ 

Below is an introduction to HTML elements and tags that we will use in todays workshop:


## HTML elements
A HTML element is defined by a start tag, some content and an end tag

```html
 <tagname> Element content goes here ... </tagname>
```

### h1
  
```html
 <h1> ... </h1>
```

'h' for heading and this element defines a large heading (the h2 element defines a slightly smaller heading, h3 smaller again etc.).

### p
  
```html
 <p> ... </p>
```

'p' for paragraph, the p element defines a paragraph.

### div
  
```html
 <div> ... </div>
```
The div tag creates a section or container in HTML. It groups together other elements, allowing you to apply styles and organize your page content more effectively. Think of it as a way to add structure and order to your web design.


### title
  
```html
 <title> ... </title>
```

The title element is within the <head> and this text will appear in the title of your browser.


### html
  
```html
 <html> ... </html>
```

The html is always at the beginning of html content and /html is always at the end. So, basically the entire content of any website wil be found between these two tags.

### head 
  
```html
 <head> ... </head>
```

The head is an element that contains meta information about the document but note, is not displayed on the screen (the page configuration details).

### body
  
```html
 <body> ... </body>
```

The body contains everything that is displayed on the web page, a container for all the visible contents, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.

### link
  
```html
 <link> ... </link>
```
The link tag that we are going to use is typically used to link external style sheets. When linking in html, typically the a tag is used to link to an external page and you can find more information at: https://www.w3schools.com/tags/tag_a.asp 

### button
  
```html
 <button> ... </button>
```
The button tag defines a clickable button. https://www.w3schools.com/tags/tag_button.asp

### script
  
```html
 <script> ... </script>
```
The script tag points to a script file, in our example the javascript file. https://www.w3schools.com/tags/tag_script.asp

In our project below, this script tag will link the html file with the javascript file.


Notes: 
* <!DOCTYPE html> is not a HTML tag, it only declares the document type (informing the browser that the document type).
* The <html> is always at the beginning of html content and </html> is always at the end. So, basically the entire content of any website will be found between these two tags.
* The <head> is an element that contains meta information about the document but note, is not displayed on the screen (the page configuration details).
* The <body> contains everything that is displayed on the web page.
* The <title> element is within the <head> and this text will appear in the title of your browser.
* The <link> element is used for connecting your webpage to various resources such as CSS files (for styling) and JavaScript files (for added functionality). This practice is essential for creating dynamic, interactive, and well-designed websites.


## Let's practise some HTML

In the HTML panel in JSFiddle we are going to introduce some the HTML from above. 

Here's an example of basic HTML file. We invite you to recreate this in the HTML panel in your JSFiddle sandbox

```html
<!-- HTML code to display 'Hello, World!' -->
<head></head>
<body>
  <h1>Hello, World!</h1>
</body>
```

The first line introduces us to a comment in HTML. Comments are used in every language and this is how it looks in HTML. Note the exclamation mark at the beginning tag but not the end tag.

We are using the head and body elements, and as explained above, we populate the body to display content. Within the body we add a header, h1 in this example. We add the content 'Hello, World!' to our header. Note the indentation of the header here.

Once you have this replicated in your HTML panel on JSFiddle, click 'Run' on the top right hand corner of the sandbox and observe the Result Panel in the bottom right hand corner.

### Try it yourself
* Play with the content of the header and run the application again.
* Change the comments, delete a line, change the header size, play around with the code and click Run to see what happens.
* Create a div, button and input field

The cool HTML stuff we are going to utilise here are a div section where we will display some data about weather, a search button (where we can search a location), and this will require a place to input the data.

```html
<html>

<head>
    <title>Coding Workshop Weather Application</title>
</head>

<body>
 <div class="container">
      <div class="input">
         <input type="text " class="inputValue" placeholder="Enter Location">
         <button class="button"><i class="fas fa-search"></i></button>
      </div>

      <div class="displayWeather">
         <h1 class="temp">----°C</h1>
         <p class="humidity">---</p>
         <p class="wind">---</p>
         <h4 class="desc">---</h4>
         <p class="icon">---</p>
      </div>

    </div>
</body>

</html>
```

Take a moment to think about apps on your phone that have some of these elements.

### Before we move onto CSS, add the following to the HTML panel on your local JSFiddle

Note the elements we have explained above. 


```html
<html>

<head>
  <!-- LINK TO CSS-->
  <link rel="stylesheet" href="./api.css">

  <!-- LINK TO FONT AWESOME IN ORDER TO DISPLAY SEARCH ICON-->
  <link rel="stylesheet" 
        href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/css/all.min.css"
        integrity="sha512-HK5fgLBL+xu6dm/Ii3z4xhlSUyZgTT9tuc/hSrtw6uzJOvgRr2a9jyxxT1ely+B+xFAmJKVSTbpM/CuL7qxO8w=="
        crossorigin="anonymous" />

  <!-- LINK TO GOOGLE FONTS, FONT BRICOLAGE GROTESQUE -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Bricolage+Grotesque:opsz,wght@12..96,200..800&display=swap" rel="stylesheet">

  <title>Coding Workshop Weather Application</title>
</head>

<body>
 <!-- LINK TO JAVASCRIPT FILE -->
 <script src="./api.js"></script>

 <div class="container">
    
   <div class="showWeather">
     <h2>WHATS THE WEATHER LIKE?</h2>
   </div>    

   <div class="input">
     <input type="text " class="inputValue" placeholder="Enter the Location">
     <button class="button"><i class="fas fa-search"></i></button>
   </div>

   <div class="showWeather">
     <h2 class="temperature">----°C</h2>
     <p class="humidity">---</p>
     <h3 class="windSpeed">---</h3>
     <p class="description">---</p>
     <img class="icon" />
     
   </div>

 </div>
 
</body>

</html>
```

If you wish to learn more about HTML, check out https://www.w3schools.com/html

The link to the Google Fonts we worked with is here: https://fonts.google.com/selection/embed and to learn more about how to work with this Google Fonts API, check out: https://developers.google.com/fonts/docs/css2


 - - - -

# CSS

CSS (Cascading Style Sheets) is the language used to style the appearance of web pages. While HTML is used to describe the structure and content of a web page, CSS is used to control it's visual presentation.

The CSS is really a place where you can make the look and feel of the app your own. Feeling eager? After the workshop play around with this file. https://www.w3schools.com/css/ offers lots of great resources to learn more about CSS. We will be only introducing this during the workshop.

### body
  
The <body> element is a crucial part of your HTML document. It wraps all the visible content of the web page, such as text, images, and other elements. By applying styles to the <body>, you can set default styles that affect the entire page. CSS is laid out a little different to HTML. 

For example:
```css
 body{
   font-family: 'Raleway', sans-serif;
   background-color: #FFFF00;
 }
```

Observe the curly brackets, semi-colons, more indentation and US-English when spelling 'color'. If you are keen to expand you CSS knowledge, be sure to check out https://www.w3schools.com/css .

### Try it yourself
* Try another font on line 2
* Lookup another background HEX color code from the Color Pickere here: https://htmlcolorcodes.com/


### Before we move onto Javascript, add the following to the CSS panel on your local JSFiddle
```css
body{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    margin: 0;
    background-image: url('https://plus.unsplash.com/premium_photo-1680339680481-edd39aa0a521?q=80&w=3328&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D');
    background-repeat: no-repeat;
    background-size: cover;
}

.container {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    width: 100%;
    max-width: 450px;
    margin: 1em;
    padding: 2em;
    border-radius: 24px;
    background: rgb(234 234 234);
    background: #000000d0;
    color: white;
}

.input > input {
    border: none;
    outline: none;
    padding: 0.3rem;
    border-radius: 18px;
    color: rgb(255 255 255);
    background: #7c7c7c2b;
    font-family: 'Bricolage+Grotesque', sans-serif;
}

button.button {
    border: none;
    width: 29px;
    padding: 6px;
    border-radius: 20px;
    background: #7c7c7c2b;
    color: white;
    font-family: 'Bricolage+Grotesque', sans-serif;
    transition: (.5s);
}

button.button:focus{
    outline:none;
}

button.button:hover{
    border: 1px solid rgb(122, 112, 112) 
}

.displayTitle{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    font-family: 'Bricolage+Grotesque', sans-serif;
}

.showWeather{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    font-family: 'Bricolage+Grotesque', sans-serif;
}
```




## Let's practise some CSS

Add the code snippet above to the CSS panel in JSFiddle and observe the changes in the Result Panel after clicking 'Run'.

So lets do this!


 - - - -


# JAVASCRIPT

Bringing our focus to the bottom left hand panel of our JSFiddle, our javascript will go here. 

Sound the trumpets 🎺🎺🎺🎺🎺 - this is the important part of our tutorial today 🥳. 

This is where we will go and fetch all the weather data. In order to retrieve the weather data from a server, we need an API.

NB: The HTML and CSS gave us the structure and styling, but the javascript we are going to tackle now will handle all the action. And the big take away from today is introducing javascript and learning what an API is.

Note: This opportunity to work with javascript offers you hands on, relevant coding experience in todays tech world. If you are thinking of stretching further into the world of coding, gaining an introduction to javascript and understanding what an API is, will be an awesome start!

## What is Javascript?

JavaScript is a language that allows you to implement features on web pages. Where the action happens - where we create and control the content of our web page. This is known as responding to events (clicks, keystrokes etc.) to fetch and display data from external sources, and update content in real-time. Think about anything that moves, refreshes or changes on your screen. We will demonstrate this in this weather application.


## Let's learn Javascript 

### var
  
```javascript
 varx = 10;
 console.log(x);
```
A variable is a container for storing information. 
* In javascript, to declare a variable, first of all, we have to write the reserved keyword var .
* Then we have to give a name to the variable (in this example x).
* Then we add an equal sign to assign a value (in this example 10) to the variable we have just declared.
* Then, we place a semicolon to end the declaration.

If you wish to learn more see: https://www.w3schools.com/js/js_variables.asp

 - - - -

### Difference between functions and methods

Understanding the difference between functions and methods in programming in general is good thing to know. We are going to take a closer look using javascript. 

### function

A function is a block of code that is reusable - this block performs a particular task. They can take input arguements and return output values.

A function example:
```javascript
function add(x, y) {
  return x + y;
}
```
Here a function takes two parameters and returns their sum.

### method

A method are functions that are called on objects and can change or update an object properties.

A method example:
```javascript
var workshop = "coding";
var workshopUpperCase = workshop.toUpperCase();
```
Here a method is called on a string object to convert the string (coding) to uppercase. In this example the toUpperCase() is a method of the string object (workshop) that returns an uppercase version of the string.

To understand objects in javascript further, see: https://www.w3schools.com/js/js_objects.asp


### document.getElementById() and document.querySelector() 
Two of the most commonly used functions to retrieve elements from a webpage are querySelector() and getElementById().

The main difference between these two functions is the way they select elements. getElementById() works with ID attributes, and querySelector() works with any CSS selector. 

### document.getElementById()
In the example below, we create a variable called x, another called y and a third called z, and assign them values.
```javascript
var x = 4;
var y = 8;
var z = x + y;
document.getElementById("demo").innerHTML = 
"The value of z is: "+ z;
```
We are using what is known as a HTML DOM element here to change the HTML content of an element and identify it with a unique id known as,in our example, demo (_id="demo"_). 

The getElementById() part of document.getElementById() is a method.  This method returns an element with a specified value.  The getElementById() method returns null if the element does not exist. The getElementById() method is one of the most common methods in the HTML DOM. It is used almost every time you want to read or edit an HTML element.

In order to display this value, we need to add the following to the HTML panel on JSFiddle. We "output" the value inside an HTML paragraph with id="demo".
```html
<html>
<body>
  <p id="demo"></p>
</body>
</html>
```

For more information on HTML DOM elements see: https://www.w3schools.com/jsref/dom_obj_all.asp


### document.querySelector
In order to access the components we declared in our HTML file (temp, humidity, wind, and desc), so as we can manipulate them, we need to add functionality in our javascript file.  Here is what that looks like:
```javascript
// ACCESSING ALL THE HTML COMPONENTS REQUIRED TO PERFORM ACTIONS ON.
var button = document.querySelector('.button')
var inputvalue = document.querySelector('.inputValue')
var nameVal = document.querySelector('.name');
var temp = document.querySelector('.temp');
var humidity = document.querySelector('.humidity');
var wind = document.querySelector('.wind');
var desc = document.querySelector('.desc');
var icon = document.querySelector('.icon');

```
Notice the _document.querySelector_ . This is a method in JavaScript that allows you to select a single element from the HTML _document_ using a CSS selector (such as a class, id, or tag name). 

(If you have time to dig a little deeper on this, tackle the 'Try it yourself' at https://www.w3schools.com/jsref/met_document_queryselector.asp ). 


### .addEventListener

In our javascript file we add a event listener. The listener listens out for an event (something) to happen. The event in this case is the click of a button.  A event listener is associated to our button, as per this code snippet, the addEventListener() method is attaching an event handler to the button element.
```javascript

// ADDING EVENT LISTENER TO SEARCH BUTTON  
button.addEventListener('click', function(){

    // Fection data from open weather API
    fetch(`https://api.openweathermap.org/data/2.5/weather?q=${inputvalue.value}&units=metric&appid=01d5af53849e7b901e9afd60639538b8`)
    .then(response => response.json())
    .then(
        displayData)
    .catch(err => alert('Wrong City name')); 

})

```

If you observe the code carefully, the indentation highlights that we are creating another function, (within that function) - a fetch() method. Here we capture the API link (the point in our application where we reach out to the live data, the weather API). 


### fetch
To understand a fetch a little more, take a look here: https://www.w3schools.com/jsref/api_fetch.asp

The fetch() method starts the process of fetching a resource from a server (in our application, the weather data from the Open Weather Map API).  And the fetch() method will then return what's known as a promise that resolves to a response object.  

Understand what promise objects are all about, asynchronous operations etc. is beyond the scope of today's workshop but if you are interested to learn more, check out https://www.w3schools.com/js/js_promise.asp 

So, what we have created here is a button. We want our users to enter a location and click the search button to get the temperature and description and .... of that location.


***explain the change in the API link

TO DO... rename and create function display data...

```javascript
// Function to diplay weather on html document
const displayData=(weather)=>{
    temp.innerText=`${weather.main.temp}°C`
    desc.innerText=`${weather.weather[0].main}`
```

To finalise the javascript piece of the project...
```javascript
// ACCESSING ALL THE HTML COMPONENTS REQUIRED TO PERFORM ACTIONS ON.
var button = document.querySelector('.button')
var inputvalue = document.querySelector('.inputValue')
var nameVal = document.querySelector('.name');
var temperature = document.querySelector('.temperature');
var humidity = document.querySelector('.humidity');
var windSpeed = document.querySelector('.windSpeed');
var description = document.querySelector('.description');
var icon = document.querySelector('.icon');
//var img = document.querySelector('.img');


// ADDING EVENT LISTENER TO SEARCH BUTTON  
button.addEventListener('click', function(){

    // Fetching data from open weather API
    fetch(`https://api.openweathermap.org/data/2.5/weather?q=${inputvalue.value}&units=metric&appid=01d5af53849e7b901e9afd60639538b8`)
    .then(response => response.json())
    .then(showData)
    .catch(err => alert('Incorrect location')); 

})

// Function to display the  weather on html document
function showData(weather){
    temperature.innerText=`${weather.main.temp}°C`//text between curly brackets as per API
    humidity.innerText=`${weather.main.humidity}% Humidity`
    windSpeed.innerText=`${weather.wind.speed} Wind flow speed`
    description.innerText=`Description: ${weather.weather[0].main}`
    icon.src=`https://openweathermap.org/img/wn/${weather.weather[0].icon}.png`
}

    

    
```
 - - - -

### What is an API you ask?  
...
API stands for Application Programming Interface. It’s a set of rules that allows different software applications to communicate with each other. Think of an API as a bridge between your application and a service or data source. In this case, we’re using an API to fetch weather data. And it will be real, live data we are are going to get back - how cool is that. Check out https://openweathermap.org/api for more information.

Fun fact! Part of the mission of the team who run Open Weather Map is as follows... _By keeping our data open and accessible, we empower companies to face environmental challenges while staying committed to green practices._ So this gives us an understanding of why it is free. 

An API is like a restaurant menu. It tells you what you can order (the data or services) and how to place your order (how to make requests). The weather API we’re using provides weather data based on our requests, like the current temperature or humidity for a specific city.

So, did you use your phone to pay for your parking today? Or check out the weather on your phone? Make a payment to your pal on Revolut? Book an Uber?  You are using APIs every day.  They are all around us and are the essence of what developers work with on a daily basis.


### Project files

```html
<html>

<head>
  <!-- LINK TO CSS-->
  <link rel="stylesheet" href="./api.css">

  <!-- LINK TO FONT AWESOME IN ORDER TO DISPLAY SEARCH ICON-->
  <link rel="stylesheet" 
        href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/css/all.min.css"
        integrity="sha512-HK5fgLBL+xu6dm/Ii3z4xhlSUyZgTT9tuc/hSrtw6uzJOvgRr2a9jyxxT1ely+B+xFAmJKVSTbpM/CuL7qxO8w=="
        crossorigin="anonymous" />

  <!-- LINK TO GOOGLE FONTS, FONT BRICOLAGE GROTESQUE -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Bricolage+Grotesque:opsz,wght@12..96,200..800&display=swap" rel="stylesheet">

  <title>Coding Workshop Weather Application</title>
</head>

<body>
 <!-- LINK TO JAVASCRIPT FILE -->
 <script src="./api.js"></script>

 <div class="container">
    
   <div class="showWeather">
     <h2>WHATS THE WEATHER LIKE?</h2>
   </div>    

   <div class="input">
     <input type="text " class="inputValue" placeholder="Enter the Location">
     <button class="button"><i class="fas fa-search"></i></button>
   </div>

   <div class="showWeather">
     <h2 class="temperature">----°C</h2>
     <p class="humidity">---</p>
     <h3 class="windSpeed">---</h3>
     <p class="description">---</p>
     <img class="icon" />
     
   </div>

 </div>
 
</body>

</html>
```

```css
body{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    margin: 0;
    background-image: url('https://plus.unsplash.com/premium_photo-1680339680481-edd39aa0a521?q=80&w=3328&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D');
    background-repeat: no-repeat;
    background-size: cover;
}

.container {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    width: 100%;
    max-width: 450px;
    margin: 1em;
    padding: 2em;
    border-radius: 24px;
    background: rgb(234 234 234);
    background: #000000d0;
    color: white;
}

.input > input {
    border: none;
    outline: none;
    padding: 0.3rem;
    border-radius: 18px;
    color: rgb(255 255 255);
    background: #7c7c7c2b;
    font-family: 'Bricolage+Grotesque', sans-serif;
}

button.button {
    border: none;
    width: 29px;
    padding: 6px;
    border-radius: 20px;
    background: #7c7c7c2b;
    color: white;
    font-family: 'Bricolage+Grotesque', sans-serif;
    transition: (.5s);
}

button.button:focus{
    outline:none;
}

button.button:hover{
    border: 1px solid rgb(122, 112, 112) 
}

.displayTitle{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    font-family: 'Bricolage+Grotesque', sans-serif;
}

.showWeather{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    font-family: 'Bricolage+Grotesque', sans-serif;
}
```

```javascript
// ACCESSING ALL THE HTML COMPONENTS REQUIRED TO PERFORM ACTIONS ON.
var button = document.querySelector('.button')
var inputvalue = document.querySelector('.inputValue')
var nameVal = document.querySelector('.name');
var temperature = document.querySelector('.temperature');
var humidity = document.querySelector('.humidity');
var windSpeed = document.querySelector('.windSpeed');
var description = document.querySelector('.description');
var icon = document.querySelector('.icon');
//var img = document.querySelector('.img');


// ADDING EVENT LISTENER TO SEARCH BUTTON  
button.addEventListener('click', function(){

    // Fetching data from open weather API
    fetch(`https://api.openweathermap.org/data/2.5/weather?q=${inputvalue.value}&units=metric&appid=01d5af53849e7b901e9afd60639538b8`)
    .then(response => response.json())
    .then(showData)
    .catch(err => alert('Incorrect location')); 

})

// Function to display the  weather on html document
function showData(weather){
    temperature.innerText=`${weather.main.temp}°C`//text between curly brackets as per API
    humidity.innerText=`${weather.main.humidity}% Humidity`
    windSpeed.innerText=`${weather.wind.speed} Wind flow speed`
    description.innerText=`Description: ${weather.weather[0].main}`
    icon.src=`https://openweathermap.org/img/wn/${weather.weather[0].icon}.png`
}

    

```
