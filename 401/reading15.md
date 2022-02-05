# Reading: Trees

[Source](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)

Trees are read from the TOP down, the opposite of real trees.

They start with a _root_ and expand from there with _edges_ pointing towards their child nodes.

## Tree Terminology

**Node**:  
Has it's own values and references to other nodes

**Root**:  
The tree's beginning node

**K**:  
Used in a _k-ary_ tree to identify a node's maximum amount of children

Ex: In a binary tree, `k = 2`

**Left**:  
Refers to the _left_ child node in a tree

**Right**:  
Refers to the _right_ child node in a tree

**Edge**:  
The link between a parent and child node. The line or arrow in a visual.

**Leaf**:  
A node without children. Quite literally like a leaf on a real tree.

**Height**:  
Quantity of _edges_ from the _root_ to the furthest _leaf_

## Tree Traversals

"The most common way to traverse through a tree is to use _recursion_."

**Depth First**:  
Going through the _height_ of the tree

There are three methods for depth first traversal and each one changes the order we can search or print the _root_.

- Pre-order: root -> left -> right
- In-order: left -> root -> right
- Post-order: left -> right -> root

**Breadth First**:  
Going through the tree node-by-node (can be thought of as width rather than Depth First's _height_)

Traversal usually uses a _queue_ rather than call stack via recursion

**Binary vs K-ary Trees**:

Binary Trees can only have TWO children (left and right) whereas K-ary tree nodes can have MORE than two child nodes

[<<<Back](README.md)