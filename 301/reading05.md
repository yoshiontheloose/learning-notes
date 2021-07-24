# React Docs - Thinking in React

Source: (https://reactjs.org/docs/thinking-in-react.html)

---

### Start With A Mock

### Step 1: Break The UI Into A Component Hierarchy

Design a data model to map out the UI into components and subcomponents.

### Step 2: Build A Static Version in React

Create the parent/child components that will be passing props.

### Step 3: Identify The Minimal (but complete) Representation Of UI State

Figure out the minimum representation of "state" for changes in the UI.

### Step 4: Identify Where Your State Should Live

### Step 5: Add Inverse Data Flow

---

## Reading Questions

**How would you break a mock into a component heirarchy?**

Design a data model to map out the UI into components and subcomponents.  
Identify the sub/components by naming and drawing boxes around them.

**What is the single responsibility principle and how does it apply to components?**

Single responsibility principle states that a component should only do one thing and have subcomponents if it grows.

**What does it mean to build a ‘static’ version of your application?**

Creating the parent/child component library, basically a skeleton of what will need to take the props data. The only method present during this stage will be render().

**Once you have a static application, what do you need to add?**

State! The minimum state requirements.

**What are the three questions you can ask to determine if something is state?**

> "Is it passed from a parent via props?"  
> "Does it remain unchanged over time?"  
> "Can you compute it based on any other state or props in your component"

**How can you identify where state needs to live?**

- "Identify every component that renders something based on that state."

- "Find a common owner component"

- Common owner or components higher in the hierarchy chain should own state

- Make a new component home for a misfit state when no other component homes make sense for it. In the hierarchy, place it above it's common owner component

---

### Things I want to know more about

A better way to word this question used to determine state:

- "Can you compute it based on any other state or props in your component"

<br>

[State vs Props Review from Reactjs](https://reactjs.org/docs/faq-state.html#what-is-the-difference-between-state-and-props)

<br>

[<<<Back](README.md)