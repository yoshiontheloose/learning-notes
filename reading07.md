# How Javascript makes web pages more interactive page 1-24
    * access content
    * modify content
    * program rules
    * react to events

Browsers vary with inconsistencies affecting javascript devs. jQuery helps with those inconsistencies

**Script** - a series of instructions a computer can follow to achieve a goal
    * made up of step by step instructions

## Writing a script
    * Define the goal
    * Design the script
    * Code each step

_Computers need every detail_ 

Flowcharts are handy tools to fit tasks together because they show the paths between steps

# Page 74-79

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

# Functions Pages 88-94

### What is a function
Functions - allow you to group a series of statements together to perform a specific task
    * If parts of a script repeat the same task, you can reuse the function instead of repeating the same set of statements
    * functions are also a way to store the steps needed for a task 
    * function name should describe the task you are performing 
    * Calling the function - aka asking the function to perform it's task

Parameters - Pieces of info passed to a function 

Creating a function
    - declare function using "function" as a keyword   
        EX: function
    - give the function an identifier followed by parentheses ()
        EX: sayHello()
    - statements to perform task go in a code block in curly braces {}
        EX: document.write('Hello!');

        \function sayHello() {
            document.write('Hello!');
        }

Declaring functions that need parameters
    * a function that needs specific information to perform it's task
    * parameters are used like variables within the function
        In \function getArea(width, height)
        (width, height) is the parameter
    
    *Arguments - variables are more specific. The example above would have the numbers of width and height. 
