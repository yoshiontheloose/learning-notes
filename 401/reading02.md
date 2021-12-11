# Testing and Modules

## In Tests We Trust - TDD with Python

[Source](https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)

**Unit Tests** - "some pieces of code to exercise the input, the output and the behaviour of your code."

**Test-Driven Development (TDD)** - Strategically thinking about and writing tests first

Test file name and module name should be corresponding. Test file name begins with ***test_***

Ex:
> `module.py` for module
> `test_module.py` for test

Test names should represent what is being tested and what's expected

### **Structure: Arrange, Act, and Assert**

- Arrange - (Input) Organize necessary data for code to execute

- Act - Execute the code/exercite the behaviour

- Assert - (Output) Make sure the test function and expected result match

### **The Cycle**

(Red) Write a test, have it fail due to feature not being coded

(Green) Write the feature so the test willpass

(Blue) Refactor your code

First thing's first, think about the software design and break it into smaller pieces

---

## If name equals main

[Source](https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)

> `__name__==__main__`

"Every Python module has it’s __name__ defined and if this is ‘__main__’, it implies that the module is being run standalone by the user and we can do corresponding appropriate actions."

"If you import this script as a module in another script, the __name__ is set to the name of the script/module."

"Python files can act as either reusable modules, or as standalone programs."

"if __name__ == “main”: is used to execute some code only if the file was run directly, and not imported."

## Recursion

[Source](https://www.geeksforgeeks.org/recursion/)

**Recursion** - When a function calls itself (directly or indirectly)

Direct - A function calls the same function

Indirect - A function that calls another function

---

# Videos

## What on Earth is Recursion

[Source](https://www.youtube.com/watch?v=Mv9NEXX1VHc)

## Python Modules and Packages Companion Video

[Source](https://realpython.com/courses/python-modules-packages/)

---

# Bookmark/Skim

## Google for Education: Python Lists

[Source](https://developers.google.com/edu/python/lists)

## Google for Education: Python Strings

[Source](https://developers.google.com/edu/python/strings)

## Python Modules and Packages

[Source](https://realpython.com/python-modules-packages/)

## Pytest Documentation

[Source](https://docs.pytest.org/en/latest/)

## PyTest Tutorial

[Source](https://www.guru99.com/pytest-tutorial.html)

- Up to section Running tests in parallel

[<<<Back](README.md)
