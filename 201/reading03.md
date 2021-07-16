***Duckett HTML book***

# Chapter 3: Lists (p 62-73)

## List Types

***Ordered Lists*** - list items are numbered in order

- \<element> = \<ol>\</ol>

***Unordered Lists*** - list items are bulleted and have no need for an order

- \<element> = \<ul>\</ul>

***Definition Lists*** - list made up of terms and their definitions

- \<element> = \<dl>\</dl>
  - \<dt>\</dt> for term
  - \<dd>\</dd> for definition 

Lists can go in lists... lists on lists on lists
____________
______________

# Chapter 13: Boxes (p 300-329)

Use CSS to make box homes for elements. Height and Width properties determine the box dimensions.

- pixels - traditional. accurate detail. 
- percentages - helps fit to window size
- ems - text size makes box size

min-width and max width, min-height and max-height

- control box measurements

Overflow - manages content that is larger than the box

- Hidden - hides content if it doesn't fit in box
- Scroll -  adds scrollbar to box

## Borders. _Making the box_

**border-width**: Made with pixels or these values. Each side can be different.

- thin, medium, thick

- border-top-width, border-right-width, border-bottom- width, border-left-width

**border-style**: Styled with these values

- solid | dotted | dashed | double | groove | ridge | inset | outset |

**border-color**: RGB values. Each side can be a different color.
  
- top, right, bottom, left.  
_NORTH EAST SOUTH WEST_
  
**shorthand border**: width, style, and color all on same line. A family in a single property

## Margins. _Space outside the box_

- traditional value is pixels.
- can use percentages or ems.
- Each side can be different. Margin-top, etc. (NESW/clockwise)
- shorthand

## Padding. _Space inside the box_

- traditional value is pixels.
- can use percentages or ems.
- Each side can be different. Padding-top, etc. (NESW/clockwise)
- shorthand

**specifying a box width adds padding**

## Centering Content

- Set a width for the box

- Set left and right margins to "auto"

___
***Duckett JS Book***

# Chapter 4: Decisions and Loops from switch statements on (p 162-182)

## If/Else Statements

- checks a condition. If it's true, the first code block is executed. If false, the second code block is run instead.

- EX:  
`if (score >= 50) {`  
`passgo();`  
`}`
`else {`
  `doNotPassGo();`  
`}`

## Switch Statements

- Starts with a variable called "switch value"

- Each case represents a possible value for the variable

- when switch value is met, that code will run

- lives in one code block

- has a default option that is run if no cases match

- EX: Give the level title

``` 

switch (level) {  

case 'one':
title = 'level 1';
break;

case 'two':
title = 'level 2';
break;

case 'default':
title = 'test';
break;
}
```

***Break*** (above: break;) - tells interpreter switch statement is finished and to run any code after it

**Type Coercion** - Javascript converts data types behind the scenes to complete an operation. If you use a data type Javascript doesn't expect, it tries to make sense of the operatoin instead of reporting an error. "Coerces from ome type to another."

## Truthy and Falsy Values

Due to type coercion, every value in JS can be treated if it were true or false.

Can use truthy or falsy to check if something exists or not

 Falsy | Truthy
---- | ----
false (boolean falses) |true (boolean trues)
0 (number zero) | any other number than 0. commonly number 1
'Empty String' | 'String' (string with content)
NaN (not a number) | 10/5 (number calculations)
a variable with no value assigned to it | '0', 'true', or 'false' written as a string

<br>

The presence of an object or array is usually considered truthy. Used when checking for the presence of an element in a page.

<br>

## LOOPS (p 170)  

Loops check a condition. If true, condition will check again until the condition runs false. Hence, looping.

**For Loop** - runs code a specific number of times. Uses a counter as a condition.

- The condition in a _for loop_ is make up of:  
Initialization  
Condition  
Update  

For Loop EX:  

```
for (let i = 0; i < value; i++)
```

initialization: let i = 0;  
Condition: i < value;  
Update: i++

**While loop** Condition can be other than the counter, and the code will continue to loop as long as the condition is true.

Keywords:  
Break - (break;) Ends the loop and interpreter moves onto the next statement outside the loop

Continue - stops the loop, updates, then checks condition again.

Loops with many items can make a browser page slower to load.


[<<<Back](README.md)