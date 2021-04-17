# Read-14, Code 401, 15 April 2021

## Trees

_The topmost node is called root of the tree. The elements that are directly under an element are called its children. The element directly above something is called its parent. For example, ‘a’ is a child of ‘f’, and ‘f’ is the parent of ‘a’. Finally, elements with no children are called leaves._

---

## Why Trees?

- One reason to use trees might be because you want to store information that naturally forms a hierarchy.

- Trees provide moderate access/search (quicker than Linked List and slower than arrays).

- Trees provide moderate insertion/deletion (quicker than Arrays and slower than Unordered Linked Lists).

- Like Linked Lists and unlike Arrays, Trees don’t have an upper limit on number of nodes as nodes are linked using pointers.

---

## Binary Tree

_A tree whose elements have at most 2 children is called a binary tree. Since each element in a binary tree can have only 2 children, we typically name them the left and right child._

---

## A Binary Tree node contains following parts.

- Data
- Pointer to left child
- Pointer to right child

---

## Important Terms

`1. Root`

In a tree data structure, the first node is called as Root Node. Every tree must have a root node. We can say that the root node is the origin of the tree data structure. In any tree, there must be only one root node. We never have multiple root nodes in a tree.

[root](https://www.btechsmartclass.com/data_structures/ds_images/Root.png)

---

`2. Edge`

In a tree data structure, the connecting link between any two nodes is called as EDGE. In a tree with 'N' number of nodes there will be a maximum of 'N-1' number of edges.

[edge](https://www.btechsmartclass.com/data_structures/ds_images/Edge.pngkkk)

---

`3. Parent`

In a tree data structure, the node which is a predecessor of any node is called as PARENT NODE. In simple words, the node which has a branch from it to any other node is called a parent node. Parent node can also be defined as "The node which has child / children".

[Parent](https://www.btechsmartclass.com/data_structures/ds_images/Parent.png)

---

`4. Child`

In a tree data structure, the node which is descendant of any node is called as CHILD Node. In simple words, the node which has a link from its parent node is called as child node. In a tree, any parent node can have any number of child nodes. In a tree, all the nodes except root are child nodes.

[Child](https://www.btechsmartclass.com/data_structures/ds_images/Child.png)

---

`5. Siblings`

In a tree data structure, nodes which belong to same Parent are called as SIBLINGS. In simple words, the nodes with the same parent are called Sibling nodes.

[Siblings](https://www.btechsmartclass.com/data_structures/ds_images/Siblings.png)

---

`6. Leaf`

In a tree data structure, the node which does not have a child is called as LEAF Node. In simple words, a leaf is a node with no child.

[Leaf](https://www.btechsmartclass.com/data_structures/ds_images/Leaf.png)

---

`7. Internal Nodes`

In a tree data structure, the node which has atleast one child is called as INTERNAL Node. In simple words, an internal node is a node with atleast one child.

[InternalNodes](https://www.btechsmartclass.com/data_structures/ds_images/Internal.png)

---

`8. Degree`

In a tree data structure, the total number of children of a node is called as DEGREE of that Node. In simple words, the Degree of a node is total number of children it has. The highest degree of a node among all the nodes in a tree is called as 'Degree of Tree'

[Degree](https://www.btechsmartclass.com/data_structures/ds_images/Degree.png)

---

`9. Level`

In a tree data structure, the root node is said to be at Level 0 and the children of root node are at Level 1 and the children of the nodes which are at Level 1 will be at Level 2 and so on..

[Level](https://www.btechsmartclass.com/data_structures/ds_images/Levels.png)

---

`10. Height`

In a tree data structure, the total number of edges from leaf node to a particular node in the longest path is called as HEIGHT of that Node.

[Height](https://www.btechsmartclass.com/data_structures/ds_images/Height.png)

---

`11. Depth`

In a tree data structure, the total number of egdes from root node to a particular node is called as DEPTH of that Node

[Depth](https://www.btechsmartclass.com/data_structures/ds_images/Depth.png)

---

`12. Path`

In a tree data structure, the sequence of Nodes and Edges from one node to another node is called as PATH between that two Nodes

[Path](https://www.btechsmartclass.com/data_structures/ds_images/Path.png)

---

`13. Sub Tree`

In a tree data structure, each child from a node forms a subtree recursively. Every child node will form a subtree on its parent node.

[SubTree](https://www.btechsmartclass.com/data_structures/ds_images/Subtree.png)

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-14)
