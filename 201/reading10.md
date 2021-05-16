***Duckett JS Book***

# Chapter 10: Error Handling and Debugging (p450-486)

Understanding execution contexts and stacks helps in finding an error in code

## Order of Execution  

- Order that statements are processed.
- Some tasks cannot complete until another statement or function have run

## Execution Contexts

Each statement in a script lives in one of the three:

- **Global context**: Code in the script, but not in a function. There is ONLY ONE on any page.
- **Function context**: Code run within a function.Each function has it's own function context.
- **Eval Context** (Not covered in the book): code in an internal function. No variable scope.

Global and Function contexts correspond with scope..

**Variable Scope**

- **Global Scope**: A variable declared outside a function can be used anywhere. No "var" keyword means it is global.
- **Function Level Scope**: A variable declared in a function can only be used in that function.

Two phases of activity in execution context:  

- Prepare: new scope created. variables functions and arguments created. 
- Execute: assign values to variables. reference functions, run their code. execute statements.

**Hoisting** - "preparing" all variables and functions by hoisting them to the top of the execution context.

**Variables Object** - Each execution context has an object that contains details of all variables, functions, and parameters.

**Lexical Scope** - Functions are linked to the object they were defined in. Child parent concept.

## Error Objects

Found in "Console" of the browser dev tools

***The 7 Error Object Types are on pages 460-461***

**Debugging** - process of deduction to find errors.

- Keep notes of tests and test results

## Console Methods

console.log() - checks expected values  
console.info() - general information  
console.warn() - used for warnings  
console.error() - used to hold errors  
console.group() - groups console messages together. Needs to close the group with console.groupEnd()  
console.table() - output of a table, shows objects and arrays  
console.assert() - tests a condition, only alerts when false

_Stepping over a function_: Pause script execution with "breakpoints." Set breakpoints in 'Sources' browser Dev tools by clicking on line you want to stop on.

Create a breakpoint in code with the keyword: ***debugger***

## Handling Exceptions

***Try***
***Catch***
***Finally***

try {
  // Try to execute this code  
}  
catch (exception) {  
  // If there is an exception, run this code  
}  
finally{  
  // This always gets executed  
}  

You can generate your own error when you know one might arise with:  
`throw new Error('message');` -make message as descriptive as possible.