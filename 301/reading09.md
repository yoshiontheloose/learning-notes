# Functional Programming

## Functional Programming Concepts

Source (https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

---

**What is functional programming?**

"Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data" — Wikipedia

**What is a pure function and how do we know if something is a pure function?**

"The function always returns the same result if the same arguments are passed in."

Pure functions do not depend on state, data, or change. Will not interact outside the function or have "side effects." Ex: modifying global objects or pass by reference parameter.

Additional Source (https://medium.com/@jamesjefferyuk/javascript-what-are-pure-functions-4d4d5392d49c)

**What are the benefits of a pure function?**

Easier to test

**What is immutability?**

_Unable to be changed_

If data's state cannot change after it's created, it is considered immutable.

A new object with new value must be created if you want to change it.

**What is Referential transparency?**

When a function has the same result with the same input consistently.

"pure functions + immutable data = referential transparency"

---

## Node JS Tutorial for Beginners #6 - Modules and require()

Source (https://www.youtube.com/watch?v=xHLd36QoS4k)

**What is a module?**

Parts of whole code split off into their own module based on their functionality and called when needed. (Files)

**What does the word ‘require’ do?**

Passes a required module to a global module

**How do we bring another module into the file the we are working in?**

Module needs to know which part we want available to all files that require said module.

module.exports = _the module we want returned_

**What do we have to do to make a module available?**

---

## Things I want to know more about

- A better/simpler way of defining Functional Programming.

- Recursion

<br>

[<<<Back](README.md)
