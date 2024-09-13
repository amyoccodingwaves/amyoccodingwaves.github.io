---
layout: default
---

## Coding Workshop Guide

This guide is designed for you to follow along as we step through todays workshop. 

You have a hard copy where you can take notes. Code snippets are available via this webpage as we code along together.



## Welcome!

We’re thrilled to have you join this Coding Waves Workshop! 😊 In this tutorial, we’ll guide you through the fascinating world of web technologies, revealing the different components that come together to create a web application.

This journey may feel like an adventure into the unknown — but don’t worry! You’ve already taken the brave first step by being here, and we’re confident you will do great. 🌟


## Introduction

Have you ever felt like the world is becoming more tech-driven, but you're not quite there yet? Or maybe you've thought the world of software is just too complex to dive into on your own?

Well, we’ve got some great news for you! Programming isn’t as daunting as it seems, and we’re here to show you just how fun it can be.

This tutorial won’t instantly make you a programmer — but that’s okay! Becoming skilled in this field takes time, practice, and patience. What we aim to do is show you that programming and website creation aren’t as complicated as they might appear. We’ll break things down into manageable pieces so that you won’t feel overwhelmed.

We hope to spark a Love for Tech in you, just like it did for us!


## What you will learn from this workshop?

By the end of this workshop, you’ll have created a small, functional web application. Today we will learn how to fetch data from a database up in the cloud - how cool is that!?

!(/assets/SampleApp.png)
![Branching](https://guides.github.com/assets/SampleApp.png)
![Branching](https://github.com/amyoccodingwaves/amyoccodingwaves.github.io/activities/hello-world/branching.png)


## Environment Setup

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


## HTML 

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

The html is always at the beginning of html content and /html is always at the end. So, bascially the entire content of any website wil be found between these two tags.

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


Notes: 
* <!DOCTYPE html> is not a HTML tag, it only declares the document type (informing the browser that the document type).
* The <html> is always at the beginning of html content and </html> is always at the end. So, bascially the entire content of any website wil be found between these two tags.
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

### Before we move onto CSS, add the following to the HTML panel on your local JSFiddle

The cool HTML stuff we are going to ulilise here are a div section where we will display some data about weather, a search button (where we can search a location), and this will require a place to input the data.

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

    <!-- LINK TO FONT AWESOME-->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/css/all.min.css"
        integrity="sha512-HK5fgLBL+xu6dm/Ii3z4xhlSUyZgTT9tuc/hSrtw6uzJOvgRr2a9jyxxT1ely+B+xFAmJKVSTbpM/CuL7qxO8w=="
        crossorigin="anonymous" />

    <!-- LINK TO GOOGLE FONTS -->
    <link rel="preconnect" href="https://fonts.gstatic.com">
    <link href="https://fonts.googleapis.com/css2?family=Raleway:wght@300&display=swap" rel="stylesheet">

    <title>Coding Workshop Weather Application</title>
</head>

<body>
 <div class="container">
    
      <div class="displayWeather">
        <h2>WHATS THE WEATHER LIKE?</h2>
      </div>    

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

    <!-- LINK TO JAVASCRIPT FILE -->
    <script src="./api.js"></script>
</body>

</html>
```

If you wish to learn more about HTML, check out https://www.w3schools.com/html/default.asp 

## CSS

CSS (Cascading Style Sheets) is the language used to style the appearance of web pages. While HTML is used to describe the structure and content of a web page, CSS is used to control it's visual presentation.

### body
  
The <body> element is a crucial part of your HTML document. It wraps all the visible content of the web page, such as text, images, and other elements. By applying styles to the <body>, you can set default styles that affect the entire page. CSS is laid out a little different to HTML. 

For example:
```css
 body{
   font-family: 'Raleway', sans-serif;
   background-color: #FFFF00;
 }
```

Observe the curly brackets, semi-colons, more indentation and US-English when spelling 'color'. If you are keen to expand you CSS knowledge, be sure to check out https://www.w3schools.com/css/default.asp

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
    background-image: url('https://media.istockphoto.com/id/1094795004/photo/blue-water-texture-from-hot-egypt.jpg?s=1024x1024&w=is&k=20&c=7Tjht1tT57X4bhW1Awpkulh62bhyLmFNEu1jTr6n3ac=');
    background-repeat: no-repeat;
    background-size: cover;
}

.container {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    width: 100%;
    max-width: 420px;
    margin: 1em;
    padding: 2em;
    border-radius: 14px;
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
    font-family: 'Raleway', sans-serif;
}

button.button {
    border: none;
    width: 29px;
    padding: 6px;
    border-radius: 20px;
    background: #7c7c7c2b;
    color: white;
    font-family: 'Raleway', sans-serif;
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
    font-family: 'Raleway', sans-serif;
}

.displayWeather{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    font-family: 'Raleway', sans-serif;
}
```




## Let's practise some CSS

Add the code snippet above to the CSS panel in JSFiddle and observe the changes in the Result Panel after clicking 'Run'.


```


## BELOW ARE TO BE DELETED ONCE TUTORIAL FINALISED - useful to styling 

Layout ideas below


Text can be **bold**, _italic_, or ~~strikethrough~~.


[Link to another page](./another-page.html).

There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# Header 1

This is a normal paragraph following a header. GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

## Header 2

> This is a blockquote following a header.
>
> When something is important enough, you do it even if the odds are not in your favor.

### Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
