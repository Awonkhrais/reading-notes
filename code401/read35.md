# Graphs

A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

## Common Terms

- *Vertex* - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
- *Edge* - An edge is a connection between two nodes.
- *Neighbor* - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
- *Degree* - The degree of a vertex is the number of edges connected to that vertex.

### Directed vs Undirected

- *Undirected* - A graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.
- *Directed* - A directed graph (also called a digraph) is a graph where every edge is directed. Unlike an undirected graph, a Digraph has direction. Each node is directed at another node with a specific requirement of what node should be referenced next.

### Complete vs Connected vs Disconnected

- *Complete* - All vertices are connected to all other vertices.
- *Connected* - All vertices have at least one edge.
- *Disconnected* - Some or all vertices may not have edges.

### Acyclic vs Cyclic

A cycle is defined as a path of a positive length that starts and ends at the same vertex. Hence, in a graph that cycles, a given node can be traversed through and potentially returned to as a result of subsequent traversals. On the other hand, an example of an acyclcing graph--a directed graph without cycles--would be a tree.

## Graph Representation

### Adjacency Matrix

An Adjacency matrix is represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix

Each Row and column represents each vertex of the data structure. The elements of both the column and the row must add up to 1 if there is an edge that connects the two, or 0 if there isn’t a connection.

### Adjacency List

An adjacency list is the most common way to represent graphs. It is a collection of linked lists or array that lists all of the other vertices that are connected. Adjacency lists make it easy to view if one vertices connects to another.

- We can visually see that we are working with a collection of some sort. The visual is depicting a Linked List, but you could easily make it an array of arrays if you’d like.
- Each index or node (depending on the data structure you choose to represent the adjacency list) will be a vertex within the graph.
- Every time you add an edge, you will find the appropriate vertices in the data structure and add it to the appropriate location.

## Weighted Graphs

A weighted graph is a graph with numbers assigned to its edges. These numbers are called weights. When representing a weighted graph in a matrix, you set the element in the 2D array to represent the actual weight between the two paths. If there is not a connection between the two vertices, a 0 is placed.

Within weighted adjacency lists, you must include both the weight and the name of the adjacent vertex.