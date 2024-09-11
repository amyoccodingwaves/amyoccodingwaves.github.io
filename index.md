---
layout: default
---

## Coding Workshop Guide

### This guide is designed for you to follow along as we step through todays workshop. You have a hard copy where you can take notes, and code snippets are available via this webpage as we code along together.

## Welcome!

We’re thrilled to have you join the coding waves Workshop! 😊 In this tutorial, we’ll guide you through the fascinating world of web technologies, revealing the different components that come together to create the web as we know it.
This journey may feel like an adventure into the unknown — but don’t worry! You’ve already taken the brave first step by being here, and we’re confident you’ll do great. 🌟


## Introduction

Have you ever felt like the world is becoming more tech-driven, but you're not quite there yet? Or maybe you've thought the world of software is just too complex to dive into on your own?

Well, we’ve got some great news for you! Programming isn’t as daunting as it seems, and we’re here to show you just how fun it can be.

This tutorial won’t instantly make you a programmer — but that’s okay! Becoming skilled in this field takes time, practice, and patience. What we aim to do is show you that programming and website creation aren’t as complicated as they might appear. We’ll break things down into manageable pieces so that you won’t feel overwhelmed.

We hope to spark a Love for Tech in you, just like it did for us!


## What you will learn from this workshop?

By the end of this workshop, you’ll have created a small, functional web application, one step at a time! 

............IMAGE OF FINISHED APP GOES HERE.........


## Environment Setup

One of the first tools we will use is JSFiddle. JSFiddle is a popular, browser-based development environment where you can write, edit, and run code in HTML, CSS and Javascript. These code snippets, known as "fiddles," allow you to experiment and see the results in real-time.

Navigate to the JSFiddle Workspace by typing in 
```
 https://jsfiddle.net/ 
```
in your browser


When you open JSFiddle, you will notice the workspace is divided into four sections:
*  HTML Panel: This is where you’ll write the structure of your webpage.
*  CSS Panel: Use this panel to style your HTML elements.
*  JavaScript Panel: Here’s where the functionality of your web application comes to life.
*  Result Panel: This section displays the output of your code, updating as you make changes.


## HTML 

HTML (HyperText Markup Language), is the foundation of every web page. It combines Hypertext, which connects different web pages, with Markup Language, which structures text within tags to form the building blocks of a webpage. (For more information, see https://www.w3schools.com/html/) 

* ### Understanding Tags
Tags are the essential building blocks of HTML. By mastering HTML tags, you can create well-structured and informative web page. An element in HTML consists of a start tag, an end tag, and the content in between. These elements form the structure of web pages, representing various types of content like headings, paragraphs, links, and images.
```
 example here...
```

* ### head tag
The <head> tag serves as a container for metadata (information about the document itself) and is placed between the <html> and <body> tags. Metadata isn't displayed on the page. It typically includes the document title, character set, links to stylesheets (CSS) and scripts.
The <head> tag is a container for metadata (data about data) and is placed between the <html> tag and the <body> tag. Metadata is not displayed.
Metadata typically define the document title, character set, styles, scripts, and other meta information. Used for containing the link for the other files such css file and JavaScript files.

```
 <head>Head Tag</head>
```

* ### body tag
The <body> element defines the main content of a webpage. Everything inside the <body> tag is what the user sees and interacts with in the browser. This includes text, images and links.
```
 <body>Body goes here</body>
```

* ### div tag
The <div> tag is a container in HTML. It groups together other elements, allowing you to apply styles and organize your page content more effectively. Think of it as a way to add structure and order to your web design.
```
 <div class="input"></div>
```
 This creates a container with the class name input. The class name is used for styling purposes with CSS.

* ### link tag
Linking Files in HTML
In HTML, linking files is crucial for connecting your webpage to various resources. You'll often link to CSS files for styling and JavaScript files for added functionality. This practice is essential for creating dynamic, interactive, and well-designed websites.

Here’s how you can include the CSS and JavaScript links in an HTML code snippet:
```
link example...
```

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
