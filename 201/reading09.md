***Duckett HTML Book***  
# Chapter 7: Forms (p144-175)

## Types of forms  

`<form>` - element where the form controls live

- requires an "action" attribute

Type | Desc. | Element
---- | ---- | ----
Text input | single line | `<input>`
Password input | hides passwords/text | 
Text Area | multiple lines of texts  
Radio buttons | multiple choice but one selection  
checkboxes | multiple choice, multiple selections  
drop down boxes |  ..
submit buttons |  ..
Image buttons |  submit an image
File upload |  ..




---
# Chapter 14: Lists, Tables & Forms (p330-357)





---
***Duckett JS Book***
# Chapter 6: Events (p243-292)

 Events are the browser's way of indicating when something happened (button clicks, page finished loading)

Events **"fire"** or are **"raised"**

Events **"trigger"** scripts

 Event types

- UI Events
- Keyboard Events
- Mouse Events
- Focus Events
- Form Events
- Mutation Events

**Event Handling** - steps to trigger some JavaScript code

- Select Element: select element node(s) you want the script to respond to
- Specify Event: indicate which event on selected node will trigger response
- Call Code: state the code you want to run when event occurs

## **Event Listeners** - allow one event to trigger multiple functions (p254)

- not supported in older browsers
- cannot have parentheses after the function names

```
element.addEventListener('event', functionName [, Boolean]);
```

Example above:

- `element.` is the DOM element node to target
- `.addEventListener('event', functionName [, Boolean]);` is the method
- `'event',` is the event to bind node
- `functionName` is name of function to call
- `[, Boolean]` indicates _capture_

If you need to pass arguments to a function that is called by an even handler or listener, wrap the function in an ***anonymous function***

- the anonymous function is used as the second argument
- interpreter sees parentheses after a function call, with an event you want the interpreter to wait until the event triggers it

```
el.addEventListener('blur', function() {
  checkUsername(5);               //anonymous function
}, false);
```



