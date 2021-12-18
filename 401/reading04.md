# Reading

## Classes and Objects

[Source](https://www.learnpython.org/en/Classes_and_Objects)

**Classes** - Where you create objects. An object template.

Multiple different objects of the same class (same variable and functions) can be created. Each object will have it's own copy of the class variables.

`init()` - when the class is initialized, this function is called to assign values in the class.

```markdown
class ClassName:

  def __init__(self, number):
    self.number = number
```

## Thinking Recursively

[Source](https://realpython.com/python-thinking-recursively/)

(Optional: Naive Recursion is Naive section and beyond)

**Recursive Function** - Calls itself, repeats behavior, and returns result when a condition is met. "_self referential expressions_"

Made up of two parts:

- Base case - the problem at large perspective

- Recursive case - the problem in simplified instances

Maintain state during recursion by either:

- passing updated current state to each recursive call as a/an argument/s

- keeping state in global scope

Data structures are recursive when they can be defined in terms of a smaller version of themselves

Python has a limit on how many stacks it can call. Stack overflow happens when more stack frames are used than the default call stack depth.

## Pytest Fixtures and Coverage

[Source](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)

**Fixtures** - objects that are available to all tests to share data

`pytest.fixture` - used with a function definition to define fixtures

`StringIO` - file-like object

---

# Bookmark/Skim

## Pytest Fixtures

[Source](https://docs.pytest.org/en/latest/fixture.html)

### note

**superclass** - a parent class

[<<<Back](README.md)
