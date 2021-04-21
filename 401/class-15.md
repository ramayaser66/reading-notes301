

# Trees

![](https://i.stack.imgur.com/5kJXf.gif)

concepts you  need to know:

- Node 
 A Tree node is a component which may contain it’s own values, and references to other nodes

- Root 
 The root is the node at the beginning of the tree

- K 
 A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree k equals 2

 - Left 
 A reference to one child node, in a binary tree

 - Right 
  A reference to the other child node, in a binary tree
- Edge 
 The edge in a tree is the link between a parent and child node
- Leaf 
 A leaf is a node that does not have any children
- Height 
 The height of a tree is the number of edges from the root to the furthest leaf

 ## Traversals 

allows us to search for a node, print out the contents of a tree, and so on

Note: the best practice when dealing with trees is recursion

categories of traversals:

- Depth First
prioritize going through the depth (height) of the tree first. 

methods implemented:


Pre-order
In-order
Post-order

- Breadth First 

 iterates through the tree by going through each level of the tree node-by-node

 Note: uses a queue instead recursion

 ## Pseudocode

 it utilizes a built-in queue to implement a breadth first traversal.

## Binary Tree 
Binary Trees restrict the number of children to two 
left and right 

it has no specific sorting order, which means nodes can be added into a binary tree wherever space allows

## Nodes 

Adding a node to a  binary tree 
it doesn’t matter where a new node gets added 

you can:
- fill all child spots from the top down.
find the first node that does not have all it’s children filled, and insert the new node as a child. We fill the child slots from left to right.




__________________________________________

## K-ary Trees
it contains more than 2 child nodes
K is used to represent the maximum number of children that each Node is able to have.


## Traversals in  K-ary tree
- Breadth First: 
pushing nodes into a queue, you movie down a list of children of length k, instead of checking for the presence of a left and a right child.

## Pseudocode in  K-ary tree

check a list of children instead of a left and right child properties.





