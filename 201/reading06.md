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

### Accessing an object (p103)

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

    - **Document Node**

    - **Element Node**

    - **Attribute Node**

    - **Text Node**

Working with the DOM tree - Accessing and updating 

- Step 1: Access the elements
  * can select by id attribute, CSS selector, class name, or tag name
- Step 2: Work with those elements  

Dom queries - methods that find elements in the DOM tree.
