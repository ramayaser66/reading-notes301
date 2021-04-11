# Object-Oriented Programming

![](https://media.geeksforgeeks.org/wp-content/cdn-uploads/extends.png)



___________________________________________________________

> Objects 
they consist of state and behavior.
the state of an object is represented in variables and the behavior in methods AKA functions.


the term data encapsulation is considered a fundamental principle of  object-oriented programming which is when you hide the state of an object and all the interactions are through a method. 

>  A Class is like an object constructor or a blueprint that your objects is based on. 

Note:  The responsibility of creating and using new objects belongs to some class in the application.

> Inheritance 
Objects can have some similar data so  classes are able to inherit commonly used state and behavior from other classes.

>  Package 
 a namespace for organizing classes and interfaces in a logical manner


# Interfaces & Inheritance


## interfaces
interfaces are a reference type, they contain:
- only constants
- method signatures
- default methods
- static methods
- nested types

Method bodies exist only for default methods and static methods

- they can only be implemented by
1.  classes 
2.  extended by other interfaces.


you can use an interface by writing a class that implements the interface, it provides a method body for each of the methods declared in the interface


interfaces can be used as  Application Programming Interface (API).


## Inheritance

- subclass:
 A class that is used from another class.

- superclass 
The class from which the subclass is used. 


A subclass inherits everything from its superclass
like: 
1. fields
2. methods
3. nested classes 
4. public and protected members
5.  package-private members


Note: Constructors are not inherited by subclasses, but the constructor of the superclass can be invoked from the subclass.

inherttace allows you to:

- declare fields in the subclass 
- write a new instance method 
-  write a new static method 
- declare new methods in the subclass
- create a subclass constructor that invokes the constructor of the superclass

