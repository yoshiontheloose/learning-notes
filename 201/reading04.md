***Duckett HTML book***

# Chapter 4: “Links” (p 74-93)  

Links - Created by using `<a>`, closes with `</a>`  
Use `href=` attribute in opening tag to specify the page to link  
_Link Text_ - text between open and close tag, displays on site  

**URL** - Uniform Resource Locator

- **Absolute URL**: starts with domain name, can add a page path on
- **Relative URL**: "Shorthand" way of telling browser where to find files. Best to use when linking within own site.
  * Does not need domain name when linking to pages on the same site.
  * Uses files/folders from on computer
  * Relative Link Types - Page 84

Directory Structure  

- Root folder - Main folder
- Directories - Folders on a website
- URLs are used when linking other sites and images onto your own site

Email Links - Direct links to a specified email address.

- mailto: then the desired email address.
- `<a href="mailto:emailaddress@email.com">Email Person</a>`

Opening a link in a new window - target attribute: _blank

- Use when opening a window to a new website
- Generally avoided, but inform users of new window opening if used

Linking to parts of the same page:  
longer pages with multiple sections can contain section links.  

- Use the "id" attribute.
- value of id attribute starts with letter or underscore.
- no two id can be the same.  

---
# Chapter 15: “Layout” (p 358-404)

CSS treats each HTML element as if it's in it's own box.

- **Block level element**: Starts on a new line. Main building blocks of a layout.
  * Ex: `<h1> <p> <ul> <li>`
  
- **Inline element**: Flow between surrounding text.
  * Ex: `<img> <b> <i>`

- **Containing element/parent element**: A block level element containing other block level elements.
  * Ex: `<div> <body>`

## Positioning

Specify positioning scheme in css by using `position:` property.  

*(Think of the image on Word with the dog)*

**Normal Flow** - Default. Straight. Does not need to be specified. (`position: static` if it did. 

**Relative Positioning** - Shifted with TRBL offset properties. Does not affect position of surrounding elements.

**Absolute Positioning** - Taken out of normal flow. Moves with the scroller. Does not affect surrounding elements.

**Fixed Positioning** - Form of absolute positioning. positions in relations to the browswer window. Uses TRBL offset properties. 

**Floating Elements** - Far left or right of a containing box. Becomes a block level element. Text flows around it. 

_Use the "width" property for how wide the floated element should be!_

  - Commonly used to float boxes next to each other. Height of box can affect where the element sits.
  - `clear:` - says that no element in the same containing box should touch the left or right sides.
    *left, right, both, none

**z-index** - "stacking content." Used if boxes overlap. Similar to "bring to front" and "send to back."

Creating multi-column layouts with floats:

- use a `<div>` element to represent each column. Can be nested. `<div class="column1of2">`
- Width - sets width of columns
- Float - positions columns next to each other
- margin - makes a gap between columns

**Standard page size - 960-1000 pixels wide**
Top 600 pixels to tell what site is about. 

**Fixed Width Layouts**  
Measurements in pixels. Size stays the same.

**Liquid Layouts**  
Measurements in percentages. Size stretches or shrinks.

Grids help structure the page.  

---
***Duckett JS book***

# Chapter 3: “Functions, Methods, and Objects” (p 86-99)

## Functions

Functions let you group statements together to perform a certain task. Code organizers.

- Used when parts of a script repeat the same task.

_"Calling a function"_ - asking the function to perform.

**Parameters** - Pieces of information passed to a function. (in parentheses).

- EX: function getArea(width, height)  

Curly braces indicate statements that perform the task. Steps or _statements_ for a function are packaged in a **code block** aka curly braces {}. NO semicolon before or after them.

**Return Value** - Response from a function when you expect it to return an answer. Interpreter leaves the function when return is used.

_"Declaring a function"_ - function keyword followed by the name you give. (p 90, 91)

Declaring a function and giving it a name allows the developer to call and use that function later in the code.

Function name is also known as an _Identifier_.

**Arguments** - Function that needs information. Has parameters. Can be values or variables. (p 93)

**Function Declaration** creates a function that you can call later in the code. Must have a name.

**Function Expression** - A function where the interpreter would expect to see an expression. Name is usually ommitted.

- **Anonymous functions** - functions with no name but are executed.

**Immediately invoked function expressions** (IIFE)

- not given a name, executed once the interpreter comes across them.
- used for code that only needs to run once within a task.

## Variable Scope
**Local Variables** - aka "function level." Variable created inside a function, can only be used in that function.

**Global Variables** - variable created outside a function. Can be used anywhere within the script. Use more memory.

Methods are the same as funtions, except they are created inside an object.

---

# Article: Pair Programming 
Source: [https://www.codefellows.org/blog/6-reasons-for-pair-programming/]  

## Pair Programming - Collaboration on one workstation between two developers.

**Driver** -  Writer. Handles the keyboarding.

**Navigator** - Editor. Does not write the code.

Four basic yet important skills developers utilize:

- Listening - Open ears for guidance from others
- Speaking - Explain what the code does with correct terminology
- Reading - Read code written by others
- Writing - Write code

### Why Pair Programming?

- _Greater Efficiency_
- _Engaged Collaboration_
- _Learning From Fellow Students_
- _Social Skills_
- _Job Interview preparation_
- _Work Environment preparation_

Both teammates can learn from each other!


[<<<Back](README.md)