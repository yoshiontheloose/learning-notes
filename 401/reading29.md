# Graphs

[Source](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/graphs.html)

**Graph**: Non-linear data structure. `vertices` or `nodes` connected by `edges`.

**Vertex** - aka `node`. Data object with 0 or more adjacent vertices.

**Edge** - connection between two nodes

**Neighbor** - adjacent nodes, connected with an edge

**Degree** - quantity of edges connected to a vertex

## Directed vs Undirected

**Undirected Graph** - Edges in the graph are "bi-directional." Connected nodes(vertices) have no directions.

**Directed Graph** - aka "diagraph." Edges are directed and nodes have a specified node to be referenced next.

## Complete vs Connected vs Disconnected

**Complete Graph** - All nodes are connected to other nodes

**Connected Graph** - All nodes have at least one edge/are connected to another node.

**Disconnected Graph** - Some nodes or at least one node does not have an edge.

## Acyclic vs Cylic

**Cycle** - When a node can be traversed through and end up back at itself

**Acyclic Graph** - aka "DAG", represented as a tree. A directed graph without cycles.

**Cyclic Graph** - A graph with cycle(s).

## Graph representation

**Adjacency Matrix** - 2-D array where each row and column represent each vertex. If there is an edge, the number is 1 or greater, if no edge, the number is 0.

- Sparse graph: few connections

- Dense graph: many connections

**Adjacency List** - "a collection of linked lists or array that lists all of the other vertices that are connected."

## Weighted Graphs

**Weights** - Edges in a weighted graph that have numbers assigned to them

---

</br>

[<<<Back](README.md)