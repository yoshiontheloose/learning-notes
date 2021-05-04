# Javascript Book Pages 43-69

How HTML, CSS, and Javascript fit together

    *\<html> - content layer. What is on the page
    * {css} - presentation layer. How the page looks
    * javascript () - behavior layer. How the page behaves

"Progressive enhancement" - using all three of these forms, a popular approach to building web pages 

## Creating a basic Javascript

JS file is a text file - it's extension is .js  

Linking to an HTML page: use the \<script> element to tell the browswer it is there

src attribute says where the JS file is stored
*  \<script> src="file.js">\</script>

most scripts added before the closing \</body> tag

HTML source code of a page will not be changed by the JS

## Statements

**Script** - series of instructions that a computer can follow one by one

**Statement** - individual instruction/step from a script
* Each one starts on a new line and ends with a semicolon
* Can be organized into _"code blocks" AKA curly braces

**Comments** - you can/should explain what your code does
* **Multi-line comments** - a comment for code that spans over one line of code
    * Starts with /* and ends with */
    - EX: \/*this code does this thing*/
* **Single line comments**
    * Use // to make a comment on a single line of code
    * Will not be processed 
    * used for short descriptions of what the code is doing

## Variables - stores info that you specified so the script can do its job. "short term memory"
* data stored in a variable can change each time a script runs  
    * EX: width x height = area
        - the measurements for width and height can vary.
        - Variables are used to to remember those values
        - similar concept to algebra

## Declare the variable

var - variable keyword, creates the variable
    variable name - sometimes called an "identifier"

EX: var quantity;
        quantity is the variable name

    Variable names longer than one word 
         - first word is all lowercase, all words after that must have their first letter capitalized
         - referred to as "camelCase" ...which is also a good example of names longer than one word
    
    Name should describe the kind of data the variable holds.
    Keywords cannot be used as variable name.
    Case sensitive.
    Do not use same word twice in a name.
    Name must begin with a letter, dollar sign $, or underscore _
    
_When declaring a variable in JS, you do not need to specify what type of data it will hold_

## Assigning a value to the variable 

_Assignment operator_ - the equals sign =
* says that you will assign a value to the variable
* also used to update the value given to a variable
* Until you have assigned a value to a variable, the value is referred to as **_undefined_**

* Once a value has been assigned to a variable, you can use the variable name to represent that value

## Data types

JS distinguishs between numbers, strings, and booleans

**Numeric data type**
* handles numbers
* tasks that involve calculating sums, use numbers 0-9, no commas
* numbers are also used for tasks like determining the screen size, moving element position, or setting amount of time an element should take to come in

**String Data Type**
* consists of letters and other characters
* enclosed in quotes. can be single or double quotes but in their rightful pairing
* Used when working with any type of text
* frequently used to add new content into a page
* can contain HTML markup


**Boolean Data Types** 
* can only be: True or False
* Helpful when determining which part of a script should run
* used when your code can take more than one path

_Escaping_ the quotation characters - backslash before any type of quote mark appearing within the string. Makes quotations inside a string "disappear" so the interpreter knows it is part of the string rather than the end of it. 

Types of selectors 
    [source](https://www.w3schools.com/css/css_selectors.asp)

**Expression** - evaluates into a single value
    *Expressions that only assign a value to a variable
        - A variable needs to be given a value to be useful
    * Expressions that use two or more values to return a single value

**Operators** - Allow programmers to create a single value from one or more values
    * Expressions rely on operators
### Types of operators
    * Assignment operators
    * Arithmetic operators 
        - multiplication and division before addition and subtraction ...basic algebra stuff
    * String operator
        - the + symbol
        - **Concatenation** - two or more strings joined together to make one new string 
        - you cannot perform addition operations on strings
    * comparison operators
    * logical operators