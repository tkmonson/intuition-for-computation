# Data Structures and Algorithms

In order to succeed in solving technical DS&A interview problems, you should go through the following steps:

1. Categorize the problem. Which data structures are applicable? Which algorithms are applicable?

## (Abstract Data Types and) Data Structures

### List

* Linked List

### Tree

### Map

### Graph

Three common ways to represent a graph:

1. **Edge list** - an array of objects containing the IDs of the vertices on which the edges are incident. Weighted edges can be expressed by including a third number (e.g. [V1,W,V2]).

2. **Adjacency list**

3. **Adjacency matrix**

Common graph problems:

* Find if a cycle exists in the graph. This is equivalent to determining if a **topological ordering** is possible and to determining if the graph is a **directed acyclic graph (DAG)**.
    
    * A **topological sort** for a DAG is a linear ordering of vertices such that for every directed edge [u,v], vertex u comes before vertex v.

    * The solution is to perform a DFS on the graph; return false if you arrive at a vertex you already visted, true otherwise.

### Stack

### Queue

## Algorithms

### Dynamic Programming (DP)

DP is a method of solving a complicated problem by breaking it into simpler subproblems using recursion. For DP to be a viable solution method, the problem must have:

1. **optimal substructure** (the optimal solution must be obtainable by combination of optimal solutions to subproblems); and

2. **overlapping subproblems** (the solutions to subproblems can be reused in later computations).

DP can be done either:

1. **top-down** (start with the complicated problem, break it into subproblems, solve those subproblems recursively, store their solutions in a cache for later use); or

2. **bottom-up** (start with the simplest subproblems---the base cases---and use their solutions to solve progressively larger problems until you get to the original complicated problem).

The Dijkstra, Bellman-Ford, and Floyd-Warshall algorithms all use DP.
