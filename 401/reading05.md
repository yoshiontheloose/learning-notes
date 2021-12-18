# Reading

## Big O: Analysis of Algorithm Efficiency

((Up through the section titled “Linear Complexity Growth”)

[Source](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/big_oh.html)

**Big O() Notation** - Describes the _worst case_ efficiency of an algorithm or function when it performs it's job

Factors of evaluation for the Big O():

- Running Time (time efficiency/complexity)
  
  - "amount of time a function/algorithm needs to complete"

- Memory Space (space efficiency/complexity)

  - "amount of memory resources that a function/algorithm uses to store data and instructions"

**4 Key Areas of Space and Time analysis:**

- _Input Size_

- _Units of Measurement_

- _Orders of Growth_

- _Best Case, Worst Case, and Average Case_

**A closer look: Input Size** -

The size of each parameter value impacts the running time and memory space. Higher numbers and arrays/lists as a parameter and their quantity of elements increase input size.

**A closer look: Units of Measurement** -

Three measurements of time to quantify Running Time:

1.) _Milliseconds_

- run-time. from start to finish of a function execution

2.) _Operations_

- quantity of code lines from start to finish of a function execution

3.) _Basic Operations_

- operation with the longest running time. Usually in the inner most loop

Four Sources of Memory Usage to quantify Memory Space. Amount of space needed to hold:

1.) _Code for the Algorithm_

2.) _Input Data_

3.) _Output Data_

4.) _Working Space/Stack Space_

Space Complexity and Time Complexity are to be analyzed separately because they are measured differently. Space is less of a concern than time with today's machines.

**A closer look: Orders of Growth** -

The increase in _Running Time_ or _Memory Space_

*Efficiency Notation Chart from Source*

![Efficiency Notations](../401/EfficiencyNotations.png)

**A closer look: Best Case, Worst Case, and Average Case** -

**Big O(oh)/Worst Case:** "upper bounds" of _Time_ and _Space_

**Big Omega/Best Case:** "lower bounds" of _Time_ and _Space_

**Big Theta/Average Case:** "tight bound" of _Time_ and _Space_

---

## Linked Lists

[Source](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html)

This reading contains many ways for creating pseudo code

**Linked List** - "sequence of `Nodes` connected/linked to each other"

Linked List Types:

- Singly - _one reference_ points to the next node in the list

- Doubly - _two references_ points to the next node and previous node

**Node** - a singular link in the list. Data for a link is stored in each node as well as a reference to the next node.

**Next** - A property with the reference to the next node. Used in traversal instead of foreach or for loops.

**Head** - The linked list's first node

**Current** - Node that is being looked at currently/where we are in the list. Allows us to move forward until the end.

**Includes** - Checks if the Linked List has a specific value or not

**Add, AddBefore, AddAfter** - used to insert nodes

---

## What’s a Linked List, Anyway pt1

[Source](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d)

**Data Structures** - Ways to organize data

**Linear Data Structures** - arranged in an order and traversed sequentially

**Non-linear Data Structures** - No arranged order, nodes may be connected to many others resulting in transversing non-sequentially

### Memory Allocation

Arrays need a single block of memory. If it needs 7 bytes, the 7 bytes will have to be together in a single block.

Linked lists can have those 7 bytes stored anywhere, they don't need to be grouped together.

**Static Data Structures** - Amount of memory is set when the structure is created.

**Dynamic Data Structures** - Does not need amount of momory to be set and it can shrink/grow.

"A node only knows about what data it contains, and who it's neighbor is"

Types of Linked Lists:

- Singly linked list - Defined previously. Ends with a node pointing to a null value.

- Doubly linked list - Defined previously. Ends with a node pointing to a null value.

- circular linked list - Has a tail node instead of a head node, beginning of the list is the node AFTER the tail node.

---

## What's a Linked List, Anyway pt2

[Source](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996)

---

<br>

### Some ideas for how you might want to teach

- Use an analogy

- Explain a detail in depth

- Use WHY, WHAT, HOW structure

- Tutorial / walk through an example

- Write a quiz

- Create a vocabulary/definition list

- Write a cheat sheet

- Create a diagram / visualization / cartoon of a topic

- Anthropomorphize the concepts, and write a conversation between them

- Build a map of the information

- Construct a fill-in-the-blank worksheet for the topic

<br>

[<<<Back](README.md)