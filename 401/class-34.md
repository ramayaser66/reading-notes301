
# Graphs

 a non-linear data structure that can be looked at as a collection of vertices  AKA nodes connected by edges 

 - Vertex, a data object that can have zero or more adjacent vertices.

 - Edge,  An edge is a connection between two nodes.
 - Neighbor,  The neighbors of a node are its adjacent nodes.
 -  Degree, The degree of a vertex is the number of edges connected to that vertex.


 ##  Undirected

a graph where each edge is undirected or bi-directional. 
It does not move in any direction.

- The connection is bi-directional. 


## Directed Graphs (Digraph)

 a graph where every edge is directed, it has a direction.
 it has arrows pointing to specific nodes.

 Each node is directed at another node with a specific requirement of what node should be referenced next.

 
## Acyclic 
 a directed graph without cycles.

 Note: A cycle is when a node can be traversed through and potentially end up back at itself. 

 - A directed acyclic graph is also called a DAG, AKA a tree.

 ## Cyclic

it has  has cycles which is a path of a positive length that starts and ends at the same vertex.



## type of graphs 

- ## Complete 

when all nodes are connected to all other nodes.


- ## Complete

 all of vertices/nodes have at least one edge.

- ## Disconnected
a graph where some vertices may not have edges.



## Graph Representation

- Adjacency Matrix
An Adjacency matrix is represented through a 2-dimensional array. 

with n vertices, then we are looking at an n x n Boolean matrix

 **sparse graph**, the case when there are very few connections.
**dense graph**,  is when there are many connections

note: an undirected graph will always be symmetric. This is not the case for a directed graph

- Adjacency List

 a collection of linked lists or array that lists all of the other vertices that are connected.

 