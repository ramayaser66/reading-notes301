# Stack 

The stack is a linear data structure that is used to store the collection of objects. 

it consists of:

- Nodes
each node reference to the next node. 


## First In Last Out (FILO)

 the first item added in the stack will be the last item popped out of the stack.



## Last-In-First-Out (LIFO)

the stack is basid on the LIFO, the last item added to the stack will be the first item popped out of the stack.
and it provieds different operations like:

- push
The push operation inserts an element into the stack, and the stack top is increased by 1, and it is an O(1) operation


- pop
pop operation removes an element from the top of the stack.
When we pop an element from the stack the value of top is decreased by 1.

When you attempt to pop an empty stack an exception will be raised.

Note: If the stack has no element is known as an empty stack. When the stack is empty the value of the top variable is -1.


1[](https://static.javatpoint.com/core/images/java-stack7.png)


## Stack Class in Java 

![](https://static.javatpoint.com/core/images/java-stack.png)

Stack is a class that falls under the Collection framework that extends the Vector class and implements interfaces
-  List 
-  Collection 
-  Iterable 
-  Cloneable 
-  Serializable.



# Queue

![](https://www.5balloons.info/wp-content/uploads/2017/06/queue.png)

_________________________________________________
Java Queue is a collection of ordered elements (Or objects) but it performs insert and remove operations differently.  
We use Queue to store elements before processing them 

it consists of: 

- Enqueue 
Nodes or items that are added to the queue. 
an O(1) operation. 

- Dequeue  
Nodes or items that are removed from the queue.
an O(1) operation. 

 it  follows the FIFO and the LILO concepts:

 - FIFO
First In First Out
 the first item in the queue will be the first item out of the queue. 


 - LILO 
 Last In Last Out

 that the last item in the queue will be the last item out of the queue.

