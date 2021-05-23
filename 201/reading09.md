***Duckett HTML Book***  
# Chapter 7: Forms (p144-175)

## Form Controls: Types of forms  

- Adding Text
- Making Choices
- Submitting Forms

`<form>` - element where the form controls live

- requires an `action=` attribute. The URL for the pageon the server to receive the info in the form
- method 
  - get: for short forms or retrieving data from the webn server
  - post: lets users upload a file, form is very long, contains sensitive data (passwords), adds or deletes info from a database


Type | Element | Attribute | Desc.  
----- | ----- | ----- | -----
Text input | `<input>` | `type='text', 'name=, maxlength`| single line
Password input | `<input>` | `type="password", name=, size=, maxlength` | hides passwords/text
Text Area | `<textarea>` closetag | - | multiple lines of texts  
Radio buttons | `<input>` | `type=radio, name=, value=, checked=` | multiple choice but one selection  
checkboxes | `<input>` | `type=checkbox, name=, value=, checked=` | multiple choice, multiple selections  
drop down boxes | `<select> + <option>` | `name=, value=, selected=` | drop down list box
submit buttons | `<input>` | `type=submit, name=, value=` | single line text input w/button
Image buttons | `<input>` | `type=image` | submit an image
File upload | `<input>` | `type=file` | file upload form w/browse and upload buttons  

Button: `<button>` Hide buttton: `type=hidden`

Label: `<label>` attribute: `for`

Date Input: `<input>`, `type=date`

**Group form controls together with `<fieldset>`. To give grouped forms a header, use `<legend>`**

<br>

### Form information is sent to the server from the browser using **key/value** pairs

`username=Ivy`  
^name=value^

<br>

---

# Chapter 14: Lists, Tables & Forms (p330-357)

Styling bullet points (aka markers)

- `list-style-type:` on css file
  - can apply to `<ol>, <ul>, <li>`

- `list-style-image: url` on css file
  - to use an image as a bullet point
  - `<ul>, <li>`

`list-style-position:` - where the bullet point sits

- `outside` - left of the text, text aligns
- `inside` - inside the text

`list-style` - bullet point's style, image, and position in any order

## Table properties

- `width` - set width of table
- `padding` - set space between borders of a cell
- `text-transform` - uppercase table header text
- `letter-spacing, font-size` 
- `border-top, border-bottom`
- `text-align`
- `background-color`
- `:hover` - highlight a table row when mouse hovers over it

Empty cell borders

- `empty-cells`
  - `show` or `hide`

Gaps between cells

- `border-spacing` - gap between adjacent cells
- `border-collapse` - ignores border spacing
- `separate` - detaches borders from each other, but obeys `border-spacing` and `empty-cells`

## Form Styling

### Styling text inputs

`font-size`
`color` - text 
`background-color`
`border`
`border-radius` - rounded corners on the form
`:focus` - changes background color
`:hover` - changes color when hovering
`background-image` 

You can also style submit buttons, fieldsets, and legends.

Forms are easier to use if the form controls are vertically aligned using CSS

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
