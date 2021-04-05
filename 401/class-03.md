# primitives vs Objects 

- primitives:
int 
booleans 
short 
long 
char 

- reference:
Integer, 
Boolean


Note: Every primitive type corresponds to a reference type.

## wrapper classes
their state can't change once the object is constructed

java converts between primitive and reference types if an actual type is different from the declared
ex: 

Integer j = 1;          
int i = new Integer(1); 


## Pros & Cons

what object should be used is based on:

1. what you are trying to achieve
2.  available memory
3. default values 


## single item memory footprint

primitive types: 
- boolean – 1 bit
- byte – 8 bits
- short, char – 16 bits
- int, float – 32 bits
- long, double – 64 bits
 - accessed fast


reference types:
- they are objects
- slow to access
- Boolean – 128 bits
- Byte – 128 bits
- Short, Character – 128 bits
- Integer, Float – 128 bits
- Long, Double – 192 bits


_______________________________________

## Exceptions
they are used to handle errors and other exceptional events.

- An exception is an event that occurs during the execution of a program that disrupts the normal flow of instructions.

- The Catch or Specify Requirement
 that code that might throw certain exceptions must be enclosed by either of the following:

 1. try, catch. 
 2. throw the exception.


 Kinds of Exceptions:
 1. checked exception.
 2. error. 
 3. runtime exception. 
 

 - Throw Exceptions

 ![](https://docs.oracle.com/javase/tutorial/figures/essential/exceptions-throwable.gif)

 All the classes are descendants of the Throwable class
 All methods use the throw statement to throw an exception. 


- try-with-resources Statement:

 a try statement that declares one or more resources.
 Note:  A resource is an object that must be closed after the program is finished with it


 - Advantages of Exceptions

 1.  Separating Error-Handling Code from "Regular" Code
 2.  Propagating Errors Up the Call Stack
 3.  Grouping and Differentiating Error Types


## Scanning

Objects of type Scanner are useful for breaking down formatted input into tokens and translating individual tokens according to their data type.

it uses white space to separate tokens.

- The ScanXan example treats all input tokens as simple String values.







