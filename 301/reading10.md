# Understanding the JavaScript Call Stack  

Source (https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4)

"_The JavaScript engine is a single-threaded interpreter comprising of a heap and a single call stack._"

Call stack is synchronous, the functions are executed from top to bottom one at a time.  

**What is a ‘call’?**

When you invoke a function. (function invocation)

**How many ‘calls’ can happen at once?**

Call stacks do _one_ thing at a time. This is referred to as, "_single threaded_"

**What does LIFO mean?**

Last In First Out.

When a function returns, the last function in a call stack is the first to come out.

**Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.**

```
function firstFunction() {
  console.log('Hello World')
}

function secondFunction() {
  firstFunction();
}

function thirdFunction() {
  secondFunction();
}

thirdFunction();
```

**What causes a Stack Overflow?**

When a function calls itself and has no exit point (**Recursive Function**)

An error will occur when the browser's max stack call is reached.

---

# JavaScript error messages

Source (https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

**What is a ‘refrence error’?**

An undeclared variable is being used. "'_blank_' is not defined"

**What is a ‘syntax error’?**

Incorrect usage of syntax

**What is a ‘range error’?**

An object has an invalid length. Out of range, so to speak.

**What is a ‘type error’?**

Incompatible accessability between a property/method and undefined type of variable.

**What is a breakpoint?**

Stops code from running at that point so you can see what happened before then

**What does the word ‘debugger’ do in your code?**

Debugger statement in code creates a breakpoint

---

## Additional Sources Provided by Reading Topic

[JavaScript errors reference on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)

---

### Things I want to know more about

What does parse mean

<br>

[<<<Back](README.md)
