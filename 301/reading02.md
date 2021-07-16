# React: Component Lifecycle Events

Source: (https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

---
## Component Lifecycle Events

- Methods (functions inside objects) you can use to define components. You can call them in a component's lifecycle  to update UI and application states.

## Phases of the Component Lifecycle

> **Mounting**

A component instance is made and inserted into the DOM

**Order of Mounting Lifecycle Events**

- static getDerivedStateFromProps()
- render()
- componentDidMount()
- UNSAFE_componentWillMount()

> ### **Updating**

A component is re-rendered when it is updated or the state changes

**Order of Updating Lifecycle Events**

- static getDerivedStateFromProps()
- shouldComponentUpdate()
- render()
- getSnapshotBeforeUpdate()
- componentDidUpdate()
- UNSAFE_componentWillUpdate()
- UNSAFE_componentWillReceiveProps()

> ### **Unmounting**

When a component is being removed from the DOM. 

_The final phase_.

**The Only Unmounting Lifecycle Event**

- componentWillUnmount()

<br>
<br>

## **constructor() in React Component**

- Constructor methods in React are called before being mounted.

- Can assign state using `this.state`

- Connect event methods to an instance

- **Do not** use `this.setState()` in a constructor. It would ignore all props updates.

### super(props)

- Call `super(props)` when component is a subclass

- _Without_ `super(props)`, the props will be undefined

<br>

## **UNSAFE Lifecycle Events**

Events that lead to bugs, not available in React 17.

UNSAFE_componentWillMount()
UNSAFE_componentWillUpdate()
UNSAFE_componentWillReceiveProps()

<br>
<br>

# Lifecycle Event Chart

![Lifecycle Event Chart](https://miro.medium.com/max/1244/1*4y9V5936WdJKaIeVPFEa3w.png)

<br>

[<<<Back](README.md)