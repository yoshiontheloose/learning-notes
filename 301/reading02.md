# React: Component Lifecycle Events

Source: (https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

---
## **constructor() in React Component**

- Constructor methods in React are called before being mounted.

- Directly assign state using `this.state`

- **Do not** use `this.setState()` in a constructor. It would ignore all props updates.

- **Do not** copy props into state unless you want to ignore the prop updates

### super(props)

- Call `super(props)` when component is a subclass

- _Without_ `super(props)`, the props will be undefined

> ### State vs Props

- Props passes data froom parent to child.
  - Child CANNOT change props
  - Handled/updated _outside_ the component.
  - Useful for displaying information in a component without hard coding

- State is data that belongs to the component, it CAN change.
  - handled/updated _inside_ the component.
  - Changes are stored in state so they render properly.

<br>

---

## Component Lifecycle Events

- Methods (functions inside objects) you can use to define components. You can call them in a component's lifecycle  to update UI and application states.

<br>

## Phases of the Component Lifecycle

> ### **Mounting**

A component instance is made and inserted into the DOM

**Order of Mounting Lifecycle Events**

- constructor()
- static getDerivedStateFromProps()
- render()
- componentDidMount()

<br>

- UNSAFE_componentWillMount()

> ### **Updating**

A component is re-rendered when it is updated or the state changes

**Order of Updating Lifecycle Events**

- static getDerivedStateFromProps()
- shouldComponentUpdate()
- render()
- getSnapshotBeforeUpdate()
- componentDidUpdate()

<br>

- UNSAFE_componentWillUpdate()
- UNSAFE_componentWillReceiveProps()

> ### **Unmounting**

When a component is being removed from the DOM.

_The final phase_.

**The Only Unmounting Lifecycle Event**

- componentWillUnmount()

<br>

---

## Defining Commonly Used Lifecycle Methods

<br>

Source: (https://reactjs.org/docs/react-component.html#componentdidmount)

### `static getDerivedStateFromProps()`

- Used if the state is dependent on changes in props
- Returns an object to update the state

### `render()`

- *Only required method* in a class component
- When called it looks at `this.props` and `this. state`
- Cannot be used to modify component state
- Does not interact with browser directly

### `componentDidMount()`

- When a component is mounted, this is invoked immediately after

- DOM node initialization

### `componentWillUnmount()`

- The cleaner upper
- Undoes/cancels anything created in componentDidMount()

### `shouldComponentUpdate()`


### `getSnapshotBeforeUpdate()`

- Captures information from the DOM before component is changed
- Returned values from this method are passed as parameters to _`componentDidUpdate()`_

### `componentDidUpdate()`

- Invoked immediately after updating

- Can do network requests here, but must compare current props to previous props

---

## **UNSAFE Lifecycle Events**

Legacy events that lead to bugs, not available in React 17.

UNSAFE_componentWillMount()
UNSAFE_componentWillUpdate()
UNSAFE_componentWillReceiveProps()

<br>
<br>

# Lifecycle Event Chart

![Lifecycle Event Chart](https://miro.medium.com/max/1244/1*4y9V5936WdJKaIeVPFEa3w.png)

<br>

---
---

### Reading Questions

---

**Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?**

- Render

**What is the very first thing to happen in the lifecycle of React?**

- constructor()

**Put the following things in their ordered sequence:**

- React
- constructor
- render
- componentDidMount
- Updates
- componentWillUnmount

**What does componentDidMount do?**

Initializes DOM nodes, loads data

**What types of things can you pass in the props?**

Any data type

**What is the big difference between props and state?**

- Props is passed into a component. Handled/updated outside the component.
- State is handled/updated inside the component

**When do we re-render our application?**

When there is a change in state or props

**What are some examples of things that we could store in state?**

Anything that needs to be changed/re-rendered

---
---

### **Additional Sources Provided by Reading Topic**
React Bootstrap Documentation (https://react-bootstrap.github.io/)

React State vs Props Video (https://www.youtube.com/watch?v=IYvD9oBCuJI)

React Docs - State and Lifecycle (https://reactjs.org/docs/state-and-lifecycle.html)

React Docs - handling events (https://reactjs.org/docs/handling-events.html)

React Tutorial through ‘Developer Tools’ (https://reactjs.org/tutorial/tutorial.html)

<br>

[<<<Back](README.md)