# React and Forms

Source: (https://reactjs.org/docs/forms.html)

<br>

HTML Form elements `(<input>, <textarea>, <select>)` update their state based on user input.

React state is updated with `setState()` and typically kept in component's state property.

Combining both HTML form elements and React state so the React state is the "single source of truth," a React component can render and update based on user input.

The input value is driven by the React state and can be passed to other UI elements or other event handlers can reset it.

**What is a ‘Controlled Component’?**

Form data handled by a React component.

**Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.**

Since the input value is driven by the React state, the state is updated with responses as soon as they are entered.

**How do we target what the user is entering if we have an event handler on an input field?**

By using a value attribute.

A value attribute is assigned so you can make a controlled component.
With multiple controlled input elements, add a name attribute to the chosen elements and the handler function chooses what to do based on the event target's value.

---

## The Conditional (Ternary) Operator Explained

Source: (https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

<br>

**Why would we use a ternary operator?**

Ternary operator AKA _Conditional operator_

To Shorten "if" statements and test if a condition is true or false (boolean value).

Ternary operators can be nested for testing multiple conditions.

Replaces the traditional "if" statement.
Traditional if statement:

```
if ( condition ) {
  value if true;
} else {
  value if false;
}
```

Ternary operator:

```
condition ? value if true : value if false
```

> WTF - What ? True : False

<br>

**Rewrite the following statement using a ternary statement:**

```
  if(x===y){
console.log(true);
  } else {
console.log(false);
  }
```

```
x===y ? 'true' : 'false'
```

---

### Additional Sources Provided by Reading Topic

React Bootstrap - Forms
[](https://react-bootstrap.github.io/components/forms/)

React Docs - conditional rendering
[](https://reactjs.org/docs/conditional-rendering.html)

<br>

[<<<Back](README.md)
