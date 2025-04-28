# HTML Basics Tutorial

Welcome to **HTML Basics**! This repository is designed to help you learn HTML from scratch. Whether you're a beginner or looking to refresh your knowledge, this tutorial will guide you through the fundamental concepts of HTML, helping you create your first web pages.

> [!NOTE]
> This tutorial is a collection my notes while I learned HTML myself and I decided to share what I learnt with everyone. Most content is minimalistic and in the form of bullet points. It's of course not perfect, so feel free to fork this repository, open issues and submit pull requests!

## Table of Contents
1. [Introduction](#introduction)
2. [The Basics](#the-basics)
3. [How Links Work](#how-links-work)
4. [The Document Object Model](#the-document-object-model)
5. [HTML5 Elements](#html5-elements)

---

## Introduction

HTML (Hypertext Markup Language) is the standard language for creating web pages. It structures the content on the web by marking up text, images, and other elements. Understanding HTML is the first step in becoming a web developer.

---

## The Basics

### What is HTML?
- Stands for HyperText Markup Language
- Helps browsers desplay viewable content
- Uses tags for annotation <>
- Tags indicates elements of website/document such as heading, lists, links

### Syntax and Semantics
- Syntax is the structure, words, symbols and punctuation of a code
- Semantics is the meaning of a code (semantic tags include header, footer...)
- Semantic elements describes its meaning to both the browser and developer

### History
- 1990:
- Way to electronically connect documents with hyperlinks (scientists needed to connect research papers)
- Common language between platforms, no device-specific markups
- Primarily text-based
- 1993:
- Mosaic, first browser that supports images arrives
- Tags no longer compatible between browsers (The Browser Wars)
- 2000 - 2005:
- Seperated content from style
- 2005 - 2008:
- Use html files with CSS

### Version History


### HTML5
- Latest version of html
- made by W3C (World Wide Web Consortium) and WHATWG
- Reduce need for external plugins
- More markup (tags) to replace scripting
- Device independent
- Tags that are not included in standard html5 are called **proprietary tags**

___

## How Links Work

### Basic Vocab

**Servers**
- Machines that hold shared info
- Always connected to network

**Client**
- Personal machines (laptop, phone)

**Networks**
- LAN (Local Area Network), many clients connected to a shared server
- WAN (Wide Area Network), connects multiple LANs. An example is the internet

### Components of a URL

**Protocols**
- http: hypertext transfer protocol (transfers html code)
- https: same as above except more secure
- ftp: file transfer protocol (transfers not just html but any type of file)
- ensures correct device communication

**Domain Name**
- The server you are connecting to (e.g. google.com, wikipedia.org)
- Mapped to an address, called IP addresses.
- **Domain Name Server (DNS)** looks up IP address based on url typed in
- Different **top-level domains** (e.g. .edu, .com, .org, .gov)

**Document**
- a specific document (e.g. contact.html)
- If none specified then return default document: index.html, which is usually homepage of websites

### Requests and Response

**Request/Response Cycle**
- When url is put in, your computer (the client) requests pages from a server and it responds with corresponding files
- Requires multiple rounds of communication in between

**Requests**
1. Browser looks up domain in DNS
2. DNS returns corresponding IP address
3. Browser sends http request to the server at that address

**Response**
1. Server finds requested files* and sends it back
2. Browser takes it and styles the html code it recieved, often repeating the steps in Requests
3. If requests can't be fulfilled, error messages will be sent back (e.g. 404, 500)

> Note: usually multiple files are sent back, rarely single files

___

## Tools & Tips

### Browsers
- Accessibility between browsers on html5 can vary
- Test your website on multiple browsers

### Text Editors
- Common text editors include TextEdit, Notepad, Sublime
- Sublime possesses most built-in functionality for html files

### Integrated Development Environments (IDEs)
- Common IDEs include VS Code, Replit
- Provides tools to help program and debug
- More advanced than text editors for coding

### Creating and Editing Files
**Naming:**
- Use a naming convention (I have chosen to use dashes)
- **No spaces**

**Editing:**
- Type ! + tab and it will give you the default html heading when you code

____

## The Document Object Model

### What is DOM?
- It is like a **tree**
- See "DOM-structure" image file

### Components of HTML Doc

**Doctype**
- Version of html used

**Head**
- Metadata - language and title (the tiny text in the tab of browsers)
- Supporting files - Javascript, CSS styling, add-ons
- Other than title, metadata is not displayed

**Body**
- Displayed content
- May be some metadata too

### Correct DOM Structure

**Coding**
- Use beginning and end tags
- Close inner tags before outer ones
- Use valid tags and attributes

**Correction**
- Use a validator to check your code

Every HTML document follows a basic structure. Here’s an example:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Basics</title>
</head>
<body>
    <!-- Content goes here -->
</body>
</html>
```
or you can check out a [demo](default-html-file-header.html).

___

## HTML5 Elements

### Attributes
- Provide additional information about element
- specified in start tag
- Come in name/value pairs

#### Display
- Most important attribute of an element
- Two types

**Block**
- Can take width and height
- Takes up the whole width of the line

**Inline**
- Cannot take width and height
- Only uses as much space as needed to contain element

#### Class
- Applies special properties to group of elements

#### Id
- Specifies unique id to one element on the page

#### Style (avoid this one)
- Specifies visual style

#### Accesskey
- A shorcut key to activate an element

#### Tab Index
- The order elements will come into focus when using tab (1 = highest priority)

### Tags
- They have beginning and end
- Some have attributes 

#### Headings (Block)
- uses "h1" to "h6" tag (most important to least important)
- Contain both syntax and semantics

#### Paragraphs (Block)
- uses "p" tag
- only contains inline elements

#### Div (Block)
- uses "div" tag
- generic section larger than paragraph
- no semantic meaning

#### Lists (Block)

**Ordered Lists**
- uses "ol" tag
- items inside use "li" tag

**Unordered Lists**
- uses "ul" tag
- items inside use "li" tag

#### Links (Inline)
- uses "a" tag
- has most common attribute href, where you put the link

#### Images (Inline)
- uses "img" tag
- has the common attributes src (source), alt (alt text), width, height, title, class

#### Line Breaks (Inline)
- uses "br" tag
- self closing tag
- inserts a new line

### Semantic Tags
- Note: **design** is very important. Clear picture of creation before coding.

#### Header (Block)
- Introductory, navigational aids: title, navigation links etc
- Not the "head" tag or the h1-h6 headings

#### Nav (Block)
- Section linking to other pages or parts within page
- Often found in header tag

#### Footer (Block)
- Contains info such as copyright, links to social media and related documents
- At bottom of a page

#### Section (Block)
- Creates sections, kinda like a div tag.

#### Aside (Block)
- Creates a space to the side of your website.

### Special Entities
- "<" = &lt
- ">" = &gt
- blank space = &nbsp
- "&" = &amp
- &copy; = &copy
- Remember: semicolon goes behind all of these

Here's a demo code consisting of many key HTML elements:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>L5 Demo</title>
</head>

<body>
    <main>
        <h1 style = "text-align: center;">This is the most important heading, centered with the style attribute</h1>
        <h2>This is the second most important heading</h2>
        <h3>This is the third most important heading</h3>
        <h4>This is the fourth most important heading</h4>
        <h5>This is the fifth most important heading</h5>
        <h6>This is the least important heading</h6>
        <br>
        <p>This is a paragraph. <a href = "https://www.w3schools.com/html/html_basic.asp">Here is a link to Html Basics</a></p>
        <ul>
            <li>This is an unordered list item</li>
            <li>It uses bullet points</li>
            <ol>
                <li>This is an ordered list inside an unordered list</li>
                <li>It is numbered</li>
            </ol>
        </ul>

        <div class="text" id="paragraph">
            <p>This is a paragraph inside a div.</p> 
        </div>

        <figure>
            <img src = "https://www.wpkube.com/wp-content/uploads/2017/09/html-chatsheet.jpg" alt = "Ultimate Html5 Cheatsheet" width = 200 height = 400>
            <figcaption>This is an Html5 cheatsheet. This caption is generated using the figcaption tag.</figcaption>
        </figure>
        
    </main>

    <footer>
        &copy;Copyright July Wu 2025.
    </footer>
        

</body>

</html>
```
or check out this [demo](L5-demo-code.html).

This is another demo consisting of more advanced HTML tags:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1>L6 Common Tags</h1>
    <h2>Horizontal Rule</h2>
    <p>Just a simple line, like below.</p>
    <hr>
    <h2>Buttons</h2>
    <button>Click Me</button>
    <hr>
    <h2>Progress</h2>
    <p>Usually used to show the completion percentage of something, like a form.</p>
    <progress value="50" max="100" width="100">50%</progress>
    <hr>
    <h2>Meter</h2>
    <p>Similar layout to progress tag.</p>
    <meter value="0.6">60%</meter>
    <meter value="0.3">30%</meter>
    <hr>
    <h2>Table</h2>
    <p>Used for creating a table.</p>
    <table>
        <tr>
            <th>First Name</th>
            <th>Last Name</th>
            <th>Age</th>
        </tr>
        <tr>
            <td>John</td>
            <td>Doe</td>
            <td>25</td>
        </tr>
        <tr>
            <td>Jane</td>
            <td>Doe</td>
            <td>22</td>
        </tr>
    </table>
    <hr>
    <h2>Form</h2>
    <p>Used for creating a form.</p>
    <form action="/submit-form" method="post">
        <label for="name">Name:</label>
        <input type="text" id="name" name="name">
        <br>
        <label for="email">Email:</label>
        <input type="email" id="email" name="email">
        <br>
        <label for="password">Password:</label>
        <input type="password" id="password" name="password">
        <br>
        <input type="submit" value="Submit">
    </form>
    <hr>
    <h2>Bdo (Bidirectional Override)</h2>
    <p>Used to override the text direction.</p>
    <p>The below order of the letters in this text will be displayed right-to-left.</p>
    <bdo dir="rtl">This text is displayed right-to-left.</bdo>


</body>
</html>
```

___

## Conclusion

Congratulations! You’ve completed the HTML basics tutorial. By now, you should be familiar with the essential building blocks of HTML and ready to start building your own web pages.

For further learning, explore more advanced topics like CSS (styling) and JavaScript (interactivity).

Happy coding!

___

### If you found this helpful, please show some love by giving this a repo a star! Enjoy programming!








