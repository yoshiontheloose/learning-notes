# Implementation: Hash Tables

## Reading

### Intro to Hash Tables

[Source](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)

**Hash**- An algorithm takes in a string and converts it to a value for a certain purpose. Determines an array index in a hashtable

**Buckets**-  The content of an index in an array for a hashtable. Can contain key/value pairs as a single index.

**Collisions**- When mulitiple keys get _hashed_ to the same location in a hashtable.

Reasons why hashtables are used:

- They hold unique values

- Dictionary

- Library

"Hashtables are a data structure that utilize key/value pairs. Every `Node` or `Bucket` has a key and value.

Hashtables store the key and retrieve the value through a `hash`.

**Hash**- encodes a key that maps to a specific location in a data structure in order to retrieve the value directly. Allows a value to be looked up in O(1) time complexity.

Hash codes turn a key into an integer. Output is determined by input. Same keys produce the same hash codes.

#### Creating a Hash

Hashtables are created from arrays.

#### Internal Methods

`Add()`- Steps to add a new key/value pair to a hashtable:

- Send key to `GetHash` method

- Determine index of where it should be placed nad go to that index

- Check for something existing in the index, Add key/value pair if nothing exists there

- When there is something that exists, add the key/value pair to the data structure in that bucket

`Find()` - takes in a key, gets the hash, goes to the specified index location

`Contains()`- accepts a key, returns a boolean about an existing key in the hashtable

`GetHash()`- accepts a key as a string, conducts the hash, returns the index of the array where the key/value pair will be placed

### Basics of Hash Tables

[Source](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)

---

## Video

### What is a Hash Table?

[Source](https://www.youtube.com/watch?v=MfhjkfocRR0)

---

## Bookmark/Skim

### Hash Table Wiki

---

</br>

[<<<Back](README.md)