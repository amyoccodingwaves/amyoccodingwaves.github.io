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

By the end of this workshop, you’ll have created a small, functional web application.

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

```
 <tagname> Element content goes here ... </tagname>
```


* ### h1
  
```
 <h1> ... </h1>
```

'h' for heading, the <h1> element defines a large heading (the <h2> element defines a slightly smaller heading, <h3> smaller again etc.).

h2, h3, h4, h5, h6

* ### p
  
```
 <p> ... </p>
```

'p' for paragraphe, the <p> element defines a paragraph.

* ### div
  
```
 <div> ... </div>
```
The <div> tag creats a section or container in HTML. It groups together other elements, allowing you to apply styles and organize your page content more effectively. Think of it as a way to add structure and order to your web design.


* ### title
  
```
 <title> ... </title>
```

The <title> element is within the <head> and this text will appear in the title of your browser.


* ### html
  
```
 <html> ... </html>
```

The <html> is always at the beginning of html content and </html> is always at the end. So, bascially the entire content of any website wil be found between these two tags.

* ### head
  
```
 <head> ... </head>
```

The <head> is an element that contains meta information about the document but note, is not displayed on the screen (the page configuration details).

* ### body
  
```
 <body> ... </body>
```

The <body> contains everything that is displayed on the web page, a container for all the visible contents, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.

* ### link
  
```
 <link> ... </link>
```

* ### button
  
```
 <button> ... </button>
```

* ### script
  
```
 <script> ... </script>
```

###### Alternative layout

| html element           | <Start tag>Element content<End tag>               |
|:-----------------------|:--------------------------------------------------|
| <h1> ... </h1>         | <h1> My first heading </h1>                       | 
| <h2> ... </h2>         | <h2> My next heading </h2>                        |
| <p> ... </p>           | <p> This is a paragraph. Enjoy reading this. </p> |
| <div> ... </div>       | <div> ... </div>                                  |
| <title> ... </title>   | <title> Jane's Webpage </title>                   |

Notes: 
* <!DOCTYPE html> is not a HTML tag, it only declares the document type (informing the browser that the document type).
* The <html> is always at the beginning of html content and </html> is always at the end. So, bascially the entire content of any website wil be found between these two tags.
* The <head> is an element that contains meta information about the document but note, is not displayed on the screen (the page configuration details).
* The <body> contains everything that is displayed on the web page.
* The <title> element is within the <head> and this text will appear in the title of your browser.
* The <link> element is used for connecting your webpage to various resources such as CSS files (for styling) and JavaScript files (for added functionality). This practice is essential for creating dynamic, interactive, and well-designed websites.







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
