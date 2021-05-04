Duckett HTML Book

# Chapter 10 Introducing CCS(p226-245)

### Understanding CSS
> _WHAT'S IN THE BOX!?!_ 

CSS allows you to create rules about each box and how it's contents are presented

HTML elements have rules that contain two parts

* **Selector**  -indicates which element the rule applies to
* **Declaration** - indicates how the elements in the selector should be styled
    - inside curly brackets
    - Made with a _property_ and a _value_ 
        * **Property** - part of the element to be changed
        * **Value** - a setting for the property
        * {property: value}  EX: {color: yellow;}

External  \<link>
  - href
  - type
  - rel

Internal \<style>
  - inside of the \<head> element


# Chapter 2 Text (p40-61)
_Markup_ - aka tags. Remember closing tags (\</tag>)

**Structural Markup**: tags for structure of the web page.
- \<h1-h6> headings, h1 biggest size
- \<p> paragraphs
- \<sup> superscript tag EX: dates. 4<sup>th</sup> written as 4\<sup>th\</sup>
- \<sub> subscript tag EX: H<sub>2</sub>0 written as H\<sub>2\</sub>0

_Empty Elements_ - no end tag
- \<br /> line break
- \<hr /> horizontal rule (a big ol break with a line)


_White Space Collapsing_ - two or more consecutive empty code lines leaves one space. two or more consecutive spaces in a line will only reflect one single space.

**Semantic Markup**: Extra info for the page, but not structure
- \<strong> browsers show bold contents
- \<em> emphasis on subtelty. browsers show italic contents.  
- \<blockquote> used for a quote that's akin to a paragraph. Usually indents the contents. Do not use this tag for indenting, it's better to use CSS for indenting. \<p> tags go inside. 
- \<q> 
- \<abbr>
- \<cite>
- \<dfn> 
- \<address>
- \<ins>
- \<del>
- \<s>


# Duckett JS Book Chapter 2 (p53-84)
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

# Variables - stores info that you specified so the script can do its job. "short term memory"
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
    
    Name should describe the kind of data the variable holds
    Keywords cannot be used as variable name
    Case sensitive
    Do not use same word twice in a name
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

## Page 74-79
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

# Chapter 4 Decisions and Loops (p145-162)