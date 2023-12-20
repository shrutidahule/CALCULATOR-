# HTML - CSS - Javascript Calculator

Today we will build a simple calculator using the technologies mentioned above. But first, we will learn a little about HTML, CSS, and Javascript before we build our calculator.

## TECHNOLOGIES DEFINED
1. **What is HTML?**
    * HTML stands for **Hyper Text Markup Language**
    * HTML elements are represented as tags and are used to build webpages.
    * Browsers **don't display HTML tags**, but use them to display content on the webpage.
2. **What is CSS?**
    * CSS stands for **Cascading Style Sheets**.
    * CSS **describes** how HTML elements look on the webpage.
3. **What is Javascript?**
    * Javascript gives us the ability to make our webpages dynamic.

![Webpage Cake](https://mdn.mozillademos.org/files/13502/cake.png)

## OBJECTIVE
1. Brief introduction to HTML, CSS, and Javascript.
2. What are HTML elements/tags?
3. How do we target HTML elements with CSS?
4. What does CSS allow us to do/change on a webpage?
5. How do we declare variables in Javascript?
6. What are Javascript functions?
7. Practice math concepts learned in class.

## OPENING EXERCISE
1. Lets download and install Sublime Text: https://www.sublimetext.com/
2. Download ZIP from https://github.com/GainorB/html-css-calculator
3. Open the starter folder with Sublime Text
4. (if necessary) Download The Unarchiver to unzip: https://theunarchiver.com/

# INTRODUCTION TO HTML

## A SIMPLE HTML DOCUMENT
```html
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```

### EXAMPLE EXPLAINED
* The ```<!DOCTYPE html>``` declaration defines this document to be HTML5
* The ```<html>``` tag is the root element of a HTML page
* The ```<head>``` tag contains meta information about the document
* The ```<title>``` tag specifies a title for the document
* The ```<body>``` tag contains the visible page content
* The ```<h1>``` tag defines a large heading
* The ```<p>``` tag defines a paragraph

## HTML TAGS
* HTML tags normally come in pairs like ```<p>``` and ```</p>```
* The first tag (opening tag) in a pair is the start tag, the second tag (closing tag) is the end tag.
* The end tag  is written like the start tag, but with a **forward slash inserted before the tag name**.

### QUESTIONS 🚨
1. What are two examples of HTML tags?
2. What is another name for the starting tag?

## HTML ATTRIBUTES
1. All HTML elements can have **attributes**.
2. Attributes **provide additional** information about an element.
3. Attributes are always specified in the **start tag**.
4. Attributes usually come in name/value pairs like: **name="value"**.
5. **THE MOST common attribute we assign are class and id. These attributes allow us to target HTML elements with CSS**.

## EXAMPLES
These are HTML tags with attributes:
```html
<div id="container"></div>
<form id="myForm"></form>

<input type="text" id="displayScreen" maxlength="10" placeholder="0" readonly></input>

<input type="button" class="button" id="btn1" value="7" onclick="display(this.value)"></input>
```

### QUESTIONS 🚨
1. Can anyone identify any HTML attributes above?
2. How do we target HTML elements with CSS?
3. Can anyone identify any new HTML tags?

# INTRODUCTION TO CSS

## A SIMPLE CSS DOCUMENT
```css
body {
    background-color: lightblue;
    color: black;
    width: 300px;
    height: 50px;
    text-align: center;
}

h1 {
    color: navy;
    margin-left: 20px;
    font-size: 20px;
    border: 2px solid red;
}
```

### EXAMPLE EXPLAINED
1. A CSS declaration **always ends with a semicolon**. 
```css
background-color: lightblue;
```
2. Declaration blocks are surrounded by **curly braces**. We use declaration blocks when we are declaring multiple css declarations.
```css
body {
    background-color: lightblue;
    color: black;
    width: 300px;
    height: 50px;
    text-align: center;
}
```
3. Each declaration includes a **CSS property name and a value, separated by a colon**.
```css
background-color: lightblue;
```

### QUESTIONS 🚨
1. How do we end CSS declarations?
2. Why do we use declaration blocks?
3. Can anyone identify any HTML tags above?

# INTRODUCTION TO JAVASCRIPT

## JAVASCRIPT VARIABLES
```javascript
var x = 5;
var y = 6;
var z = x + y;
```

### EXAMPLE EXPLAINED
1. You declare a Javascript variable with the **var** keyword.
2. Javascript variables are containers for storing data values.
3. In this example, x, y, and z, are variables:
    * x stores the value 5
    * y stores the value 6
    * z stores the value 11
4. In programming, just like in algebra, we use variables (like x, y) to hold values.
5. In programming, just like in algebra, we use variables in expressions (z = x + y).

### QUESTIONS 🚨
1. How do we declare a Javascript variable?
2. What are Javascript variables?

## JAVASCRIPT FUNCTIONS
```javascript
function myFunction(num1, num2) {
    return num1 * num2;
}
```

### EXAMPLE EXPLAINED
1. A Javascript function is a block of code designed to perform a particular task.
2. A Javascript function is defined with the **function** keyword, followed by a **name**, followed by **parentheses ()**.
3. The parentheses may include parameter names separated by commas:
**(parameter1, parameter2, ...)**.
4. The code to be executed, by the function, is placed inside **curly brackets: {}**.
5. When Javascript reaches a **return statement**, the function will stop executing.

### QUESTIONS 🚨
1. What does the function we declared above return?
2. What are the parameters in this function?
3. What is the name of the function?

# NOW, LETS BUILD THE CALCULATOR!