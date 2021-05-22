# Read-35, Code 401, 13 May 2021

## Graph

A Graph is a non linear data structure consisting of nodes and edges. The nodes are sometimes also referred to as vertices and the edges are lines or arcs that connect any two nodes in the graph. More formally a Graph can be defined as,

A Graph consists of a finite set of vertices(or nodes) and set of Edges which connect a pair of nodes.

![graph](https://ucarecdn.com/827083d1-3afc-444e-a94a-a8c239b9a76c/)

The degree is the number of edges connected to a vertex. E.g., the purple vertex has a degree of 3 while the blue one has a degree of 1.

If the edges are bi-directional, then we have an undirected graph. If the edges have a direction, then we have a directed graph or di-graph for short. You can think of it as a one-way street (directed) or two-way street (undirected).

![types](https://adrianmejia.com/images/directed-vs-undirected-graph.jpg)

### starter Code

```js
class Node {
  constructor(value) {
    this.value = value;
    this.adjacents = []; // adjacency list
}

class Graph {
  constructor(edgeDirection = Graph.DIRECTED) {
    this.nodes = new Map();
    this.edgeDirection = edgeDirection;
  }
}
```

Graphs can help to model many real-life scenarios such as airports, social networks, the internet, and so on. We covered some of the most fundamental algorithms, such as Breadth-First Search (BFS) and Depth-First Search (DFS). Also, we studied implementation trade-offs such as adjacency lists and matrix. Subscribe to my newsletter and don’t miss any of my posts because there are many other applications that we will learn soon, such as finding the shortest path between nodes and different exciting graph algorithms.

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-35)
