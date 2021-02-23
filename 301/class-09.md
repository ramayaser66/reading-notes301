

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS8KNmE0XuRbTEZcjeUoX8XNRDFcYysYM68FA&usqp=CAU)




# Functional Programming

 a way of:

 thinking about software construction by creating pure functions. It avoid concepts of shared state, mutable data observed in Object Oriented Programming.


 Note: Functional languages emphasizes on expressions and declarations rather than execution of statements.



## Pure Functions 

- It returns the same result if given the same arguments (it is also referred as deterministic)



- It does not cause any observable side effects


## Pure functions benefits

The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts:

- Given a parameter A → expect the function to return value B
- Given a parameter C → expect the function to return value D
## non-pure Functions 
- Reading Files
If it reads external files, it’s not a pure function — the file’s contents can change.

- Random number generation
Any function that relies on a random number generator cannot be pure.

-It does not cause any observable side effects 
for example, modifying a global object or a parameter passed by reference.


## Immutability

Unchanging over time or unable to be changed. 


When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.
