# Passing Functions as Props

## **React Docs - lists and keys**

Source (https://reactjs.org/docs/lists-and-keys.html)

<br>

**What does .map() return?**

- A new array of key/value for each iteration

**If I want to loop through an array and display each value in JSX, how do I do that in React?**

- Use curly braces

**Each list item needs a unique ____.**

- Key

**What is the purpose of a key?**

- "Keys help React identify which items have changed, are added, or are removed."

- They are given to the array elements.

- Using "index" as the key name is not recommended in case the order changes

<br>

---

## **The Spread Operator**

Source (https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

<br>

**What is the spread operator?**

- AKA Spread Syntax: `(...)`

- Spreads an array into separate arguments.
  - _Expands any iterable objects_

**List 4 things that the spread operator can do.**

- Copies an array

- Concatenates or combines arrays

- Using math functions

- Using an array as arguments

- Adding an item to a list

- Adding to state in React

- Combining objects

- Converting NodeList to an array

**Give an example of using the spread operator to combine two arrays.**

    const array1 = [1, 2, 3];
    const array2 = [4, 5, 6];
    const array 3 = [...array1, ...array2];

**Give an example of using the spread operator to add a new item to an array.**

    let itemStorage = [0, 1, 2];
    let newItem = 3;
    itemStorage = [...itemStorage, newItem];

**Give an example of using the spread operator to combine two objects into one.**

    let cat = {
      name: 'Beans',
      color: 'black',
    };

    let food = {
      favFood = 'salmon'
      foodType = 'crunchies'
    };

    let pet = {
      ...cat,
      ...food
    };

<br>

---

## **How to Pass Functions Between Components - Video**

Source (https://www.youtube.com/watch?v=c05OL7XbwXU)

<br>

**In the video, what is the first step that the developer does to pass functions between components?**

- Creates an increment function outside the constructor

**In your own words, what does the increment function do?**

- Updates the state of the name as it iterates

**How can you pass a method from a parent component into a child component?**

- By using props. (this.props.method)

**How does the child component invoke a method that was passed to it from a parent component?**

- By using setState()

<br>

[<<<Back](README.md)