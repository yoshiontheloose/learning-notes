# Reading

## Python Scope

[Source](https://realpython.com/python-scope-legb-rule/)

Scope as a concept: how variables and names are accessed and seen in code.

Scope of a name (of a variable/function/object etc.,) depends on where it was created in the code.

**Global Scope** - defined name is available to all code

**Local Scope** - defined name is only available to code in it's scope

**Out of Scope** - when name is out of it's code block and cannot be accessed

``` Markdown
A Note About Names:
Assignment operations (assign a name) - creating or modifying a name 

Reference/access operations (referencing a name) - grabbing the value or content of the name
```

**Namespaces** - dictionaries that map names to objects

The module's namespace stores names defined at the top level of said module.

- .__dict__

### LEGB Rule for Python Scope

**Local (function)** scope - Names defined in a function, only visible from that function's code.

**Enclosing** scope - (For nested functions) Names defined in the outer/enclosing function, visible from inner and enclosing function code

**Global (Module)** scope - defined name is available to all code (same definition above)

**Built-in** scope - contains built in names for functions, exceptions, keywords available to all code. Loaded/created automatically when a program or script is run.

---

# Videos

## Don’t be CONFUSED by BIG O notation anymore

[Source](https://www.youtube.com/watch?v=5Uqawfl0VHQ)

# Bookmark/Skim

## Rolling Dice Examples

[Source](https://artofproblemsolving.com/wiki/index.php/Basic_Programming_With_Python#Program_Example_1_3)

<br>

[<<<Back](README.md)