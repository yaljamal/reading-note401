# Graphs

A graph is a non-linear data structure that can be looked at as a collection of `nodes` potentially connected by line segments named `edges`

- terminology used when working with Graphs

1. `Vertex` also called a `node`, is a data object that can have zero or more adjacent vertices.
2. `Edge` is a connection between two nodes.
3. `Neighbor` a node are its adjacent nodes
4. `Degree` The degree of a vertex is the number of edges connected to that vertex.

## types of Graphs

1. Undirected
   is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.

2. Directed

- also called a Digraph is a graph where every edge is directed.
- Digraph has direction. Each node is directed at another node with a specific requirement of what node should be referenced next.

3. Complete
   A complete graph is when all nodes are connected to all other nodes.
4. Connected
   A connected graph is graph that has all of vertices/nodes have at least one edge.
5. Disconnected
   A disconnected graph is a graph where some vertices may not have edges.

6. Acyclic
   An acyclic graph is a directed graph without cycles.
   A cycle is when a node can be traversed through and potentially end up back at itself.
7. Cyclic
   A cycle is defined as a path of a positive length that starts and ends at the same vertex.

## Graph Representation

We represent graphs through:

1. Adjacency Matrix
2. Adjacency List
