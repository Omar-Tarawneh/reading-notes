# Read-05, Code 401, 31 Mar 2021

## Linked List

_Linked List_ A data structure that contains nodes that links/points to the next node in the list.

![node](https://miro.medium.com/max/2416/1*GOKmkucFHN_gmTMUtyC2sQ.png)

### linked list properties

- sequential nodes are connected by pointers.
- The last node points to `null`.
- A `head` pointer is maintained which points to the first node of the list.
- A linked list can grow and shrink in size during execution of the program.
- It can be made just as long as required.
- It allocates memory as the list grows. Unlike arrays, which have a fixed size.

## Advantage of linked list

- In contrast to an array, which stores data contiguously in memory, a linked list can easily insert or remove nodes from the list without reorganization of the entire data structure.

## Disadvantage of likes list

- There is no random access for any node like the array.
- Uses more memory than array.

## Type of Linked List

- Simple Linked List − Item navigation is forward only.
- **Doubly Linked List** − Items can be navigated forward and backward.
- **Circular Linked List** − Last item contains link of the first element as next and the first element has a link to the last element as previous.

## How to start typing the code

Start by defining the Node

```javascript
class Node {
  constructor(data, next = null) {
    (this.data = data), (this.next = next); // next is the pointer for the next Node
  }
}
```

Then create the Linked list class.

```javascript
class LinkedList {
  constructor() {
    this.head = null; // head is the pointer for the first node
  }
}
```

This is the first steps to implement linked list using ES6 if you want to add other feature you need to add method to add, delete or find a certain node.

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-05)
