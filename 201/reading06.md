# Understanding The Problem Domain Is The Hardest Part Of Programming
[Article Source:](https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming)  

Writer suggests learning the problem domain is the hardest part of programming. It's like a puzzle!
Take one part of the problem and fully understand that part before moving on to the next.

----
***Duckett Javascript Book***

# Chapter 3: Object Literals (p 100-105)

## What is an Object?

Objects group together a set of variables and functions to create a model of something from the real world.

Variables become known as ***properties***
  
- tells us about the object

Functions become known as ***methods***
  
- represent tasks assocaiated with the object  

Like normal variables and named functions, properties and methods still have a name and a value.

- **Key** - The name and value of properties and methods

- value of a method is always a function
-----
## Creating an object

Literal notation is the easiest and most popular way to create objects.

Setting properties - treat values like you do for variables. Strings go in quotes and arrays go in square brackets.

## Accessing an object (p103)

**Dot Notation** - name of object, period, name of property or method you want to access.

- _Member operator_ - the period

Square brackets can also access the properties or methods of an object, put them in the brackets.

- most commonly used when:
  
  - property/ method name contains special characters
  - property name is a number. Allowed to use numbers in name, but AVOID. 
  - variable is in place of property name

---
# Chapter 5: Document Object Model (p 183-242)

**DOM** - Document Object Model. Made of objects.

- Also known as an **API** (Application Programming Interface). APIs allow programs and scripts talk to each other.

The DOM states what your script can ask the browser and how to tell the browser to update the page.

## The DOM Tree (dom dom dom!)

**DOM Tree** - The way a DOM structures a model. Model is created when the browser loads a page.
  
- looks like a family tree, consists of nodes.
  
   Four main types of nodes

    - **Document Node** - Every element, attribute, or piece of text is represented by it's own DOM node.

    - **Element Node** - describes the structure of an HTML page

    - **Attribute Node** - opening tags can carry attributes. They are represented by attribute nodes in the DOM tree.

    - **Text Node** - Once you gain access to the element node, you can reach the text within the element

Working with the DOM tree - Accessing and updating

## ***Step 1: Access the elements***

  * can select by id attribute, CSS selector, class name, or tag name

### Selecting individual Element:
 `getElementById()` - Uses an elements id attribute

 `querySelector()` - Uses a CSS selector, returns the first matching element

### Selecting multiple Elements:
`getElementsClassByName()` - selects all elements with a specific value for their class attribute

`getElementsByTagName()` - Selects all elements with the specified tag name

`querySelectorAll()` - Uses a CSS selector to select all matching elements


### Traversing Between Element Nodes

`parentNode()` - Selects the parent of the current node and returns one element

`previousSibling/nextSibling` - selects the previous/next sibling from the DOM tree

`firstChild/lastChild` - Selects the first/last child of the current element


## ***Step 2: Work with those elements***  

### Access/Update text nodes

- 1. Select the element
- 2. Use `nodeValue` to get the text from the element

  `nodeValue` - lets you access or update a text node

### Work with HTML content

- `innerHTML` - allows access to child elements and text content

- `textContent` - only allows access to the text content
- `createElement(), createTextNode(), appendChild()/removeChild()` - These methods allow you to create new nodes, add notes to a tree, and remove nodes from a tree, this is called **DOM manipulation**.

### Access or Update Attribute Values

- `className` or `id` - lets you get or update the value of the class and id attributes
- `hasAttribute()` - checks if an attribute exists
- `getAttribute()` - gets value
- `setAttribute()` - updates value
- `removeAttribute()` - removes attribute

### Dom queries - methods that find elements in the DOM tree.

Script selects an element to update, interpreter has to find the element in the DOM tree.

`getElementById('one');`

If script needs to use the same elements more than once you can store the location of the element(s) in a variable. Variable stores a ***reference*** to the object in the DOM tree.  
`let itemOne = getElementById('one');`

DOM queries return one element or a NodeList.  
**NodeList** - a collection of nodes

Nodelist is where the arrays come in. To select the element you want from the NodeList, use an index number.. the [i]!

Select an element from the NodeList:

- `item()`  method - specify the index number of the element you want as a parameter.  
  use length property of NodeList to see how many items it contains.  
  The "if" statement makes a condition 

```
let elements = document.getElementsByClassName('hot')
if (elements.length >= 1) {
  let firstItem = elements.item(0);
}
```

- Array Syntax - preferred over item method, faster. NodeList is stored in a variable called elements (line 3).

```
let elements = document.getElementsByClassName('hot');
  if (elements.length >= 1) {
    let firstItem = elements[0];
}
```