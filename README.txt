# HTML-and-CSS-Crash-Course

HTML and CSS Crash Course by Net Ninja
(https://www.youtube.com/watch?v=hu-q2zYwEYs)

HTML
Hypertest Markup Language

Structure content on a web page (HTML Tags)
- open and closing tag
- HTML -> backbone of a website

CSS
Cascading Style Sheets

Style webpages to make them look better
- Design

Text editors
- Visual Studio Code
- Sublime
- Atom
- Notepad ++

Tag
Must have
<!DOCTYPE html>

<html> </html> - To start html code

Head Tag
<head> </head> - Nothing gets rendered inside the browser
  - <title> </title> - Name at the tab

Body Tag
<body> </body> - Browser
<p> </p> - Paragraph tag

Local development server > HTTP
Local server to view website

<strong> </strong> - bold tag
<em> </em> - italic
<small> </small> - smaller size

heading tags
<h1> </h1> - biggest
<h6> </h6> - least important

<ul> </ul> - unordered list
  - <li> </li> - list item

<ol> </ol> - ordered list (1, 2, 3,...)

<div> </div> - division tag
  - divide into sections
  - elements that belong together
  - would help later on when hooks are applied

<span> </span> - JS tool for hooks

<br> - line break

<hr> - horizontal rule
  - separates content
  
<img> - image tag
  - needs an attribute
  - <img src="*file*">
  - right click and get RELATIVE path
  - alt="name for screen readers"

<a> </a> - anchor tag
  - <a href="*link*"> </a>
  - href = hyperlink reference
  - styled as a link

<blockquote> </blockquote> - indent to the right
  - <blockquote cite="*link*"> - if you want to cite a website or source

<p style="color: orange;"> - example of CSS styling in a paragraph
  
<!-- *comment* --> - create a developer comment
highlight and ctrl + "/" - comment out a block of code

FORM
<form> </form>
<input type="text">
  - text input field

<input type="text" id="username">
  - id identifies the individual tag
  - can be a hook
  - can use an id for any tag

<label for="*insert id*"> </label - creates a label for an id

<label for="email"> </label>
<input type="email" id="email">
  -different in the background

<input type="*style of input*" name="*name to be addressed from the backend*" id="*reference*" value="*value of the option for server side*">*type what needs to be shown*>

<select name="" id=""> <select> - drop down box or nest
  - <option value="">*Enter what will be place din the drop down box* </option>

<textarea name="" id="" cols="" rows="" placeholder="">
  - placeholder can be used for text inputs

<input type="submit" value="Submit the form">
  - submit sends value ot the backend

required - attribute that needs the input to be filled


CSS
Style Sheet - list of CSS rules/rule sets

Selectors (div, li, etc.)
Declarations (what's inside the Selectors)

create a .css file and link it to all the pages that it will be applied in
  - place in the header
  - <link rel="stylesheet" href="*insert relative path to the .css file">
  - google any css style because there are too many to memorize them all
  - use css websafe fonts
  
Types of Elementsq
Inline Elements
  - Padding is okay but margin is only to the left and right
  - Padding goes on top of each other
  - in-line block is better

Block-level Elementsbb
  - Padding and Margin work just as intended
  - Margin goes on top of each other

User agent stylesheet - default browser style

Classes and Selectors
Class
<p class="error">
  - to reference in the CSS file, .error
  - to specify a tag with the class error, p.error
  - you can place two classes, <p class="error success">
    - to reference p.error.success

ID
  - #content{
    }
  to reference a certain div
  - div#content{
    }
 
Class -> ID
Javascript -> Class
 
decendent selector
  -space is key
  - div .error{}
  
  a[href="website"]{}
    - referencing every anchor tag with the website
  a[href*="web"]{}
    - referencing every web link that has the value of 'web'
  a[href$=".com"]{}
    - referencing every web link that ENDS with .com
    
Cascade
Inheritance
  div{
  margin: 40px;
  }
  p
  {
  margin: inherit;
  }
  
the recent (or further down) is the one that will be followed
more specific is the one that will be followed

HTML5 Semantic Tags
<main>
  - main content of a webpage

<section>
  - certain section of a webpage
  
<article>
  - makes up an article
  
<aside>
   - defines content related to soemthing else

<header>
   - header of a website (title, etc.)
 
<footer>
   - contact information, etc.
   
   
Position and Layout
Static - default
Relative - movement relative to the original position
Fixed - relative to the view port
Absoute - relative to the closest parent
Sticky - mixture of static and fixed

z index
  -layer
  -bring forward or backward
  
box-sizing
  -includes the padding
 
white-space:nowrap
  -fixes the margin and padding spacing

Pseudo classes
uses " : "
tags a class
:hover
what happens when you hover over with your mouse

:focus
what happens when you have it selected

:valid
confirm that it is valid

::first-line
change everything in the first line

::first-letter
change the first letter

::selection
what happens when you highlight or select it

::after
what you want to inject after

Responsive Design
Mobile first - prioritize content 

Add this line of code
<meta name="viewport" content="width=device-width, initial-scale=1.0")>

@media screen and (max-width:1400px){
}

