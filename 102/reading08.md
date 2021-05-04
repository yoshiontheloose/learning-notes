# Operators and Loops pages 150-151, 156, 157, 170-173, 176

## Comparison operators: Evaluating conditions

Comparison operators usually return single values of true or false

\== - is equal to 
    * compares two values (numbers, strings, or Booleans) to see if they are the same

\ != - is _not_ equal to
    * comparestwo values (numbers, strings, or Booleans) to see if they are **not** the same

\=== - Strict equal to
    * compares two values to check if data type and value are the same 

\!== - Strict _not_ equal to
    * compares two values to check if data type and value are **not** the same

\> - greater than - checks if the number on the left is greater than the number on the right

\< Less than - checks if the number on the left is less than the number on the right

\>= greater than or equal to - checks if the number on the left is greater than or equal to the number on the right

\<= less than or equal to - checks if the number on the left is less than or equal to the number on the right

**Logical operators**

Logical operators compare the results of more than one comparison operator 

Evaluated from left to right

&& Logical **And** - tests more than one condition
   
    * if both expressions are true then it is true.
    * if one is false, the whole expression is false

|| Logical **Or** - tests at least one condition
    
    * if either are true, then the whole expression returns true 
    * if both are false then the expression will return false

! Logical **Not** - takes a boolean value and inverts it
    
    * reverses the state of an expression
    * if it was false without the !, it would return as true
    * vice versa

## Loops

Loops check a condition. 
   
    * if returned true, a code block will run
    * condition will be checked again and if it is still returned as true, code block will run again
    * repeats until condition is false

Three common types of loops

**For** - when you need to run code a specific number of times
* (when you know how many times a loop will run)    
    * condition is usually a counter which is used to tell how many times the loop should run

**While** - used when you do not know how many times a code should run
    
    * condition can be something other than a counter, code will continue to loop for as long as the condition is true

**Do While**

    * similar to the "while" loop
    * Always runs the statements inside the curly braces at least once, even if the condition is false

Initialization

i - a variable that acts as the counter. 
    
    * AKA "Index"
    * only created the first time a loop is run
    * EX: i = 0;

condition

    Loop should continue to run until the counter reaches a specified number
        
        *EX: i < 10;

Update

    * Everytime the loop runs the statements in curly braces, it adds one to the counter
    * one is added to the counter using _increment operator_ (++)
    * loops can count downwards using _decrement operator_ (--)

Key difference between a _while_ loop and a _do while_ loop 
    * statements in the code block come before the condition. Statements run once whether or not the condition is met

((2 * 90) === 180) && (false && 'true')