
# Java Basics 
![](https://ucarecdn.com/6b3c5605-69ac-4ea3-b07f-18eca985f5a6/)



_____________________________________________

## Variables 

types of java variables:

- Instance Variables
 their values are unique to each object.
 they are also known as 'non-static fields' which means that fields declared without the static keyword.

 - Class Variables
 declared with the static modifier.

 - Local Variables 
a method will often store its temporary state in local variables

local variables are only visible to the methods in which they are declared, they are not accessible from the rest of the class.

- Parameters 

the signature for the main method is public static void main(String[] args).
 the args variable is the parameter to this method.

 parameters are always classified as "variables" not "fields".


 > naming 

 - Variable names are case-sensitive
 If the name you choose consists of only one word, spell that word in all lowercase letters. If it consists of more than one word, capitalize the first letter of each subsequent word.

 -  A variable's name can be any legal identifier
  — an unlimited-length sequence of Unicode letters and digits,
  - beginning with a letter,
  -  beginning with the dollar sign "$", or the underscore character "_".
  
   The convention, however, is to always begin your variable names with a letter, not "$" or "_". Additionally, the dollar sign character,

_________________________________________________


   ## Operators
   Operators are special symbols that perform specific operations on one, two, or three operands, and then return a result.


   ![](https://ucarecdn.com/4860994e-105d-456b-a98e-f3c51854830f/-/crop/478x539/214,123/-/preview/)


Note:  All binary operators except for the assignment operators are evaluated from left to right; assignment operators are evaluated right to left.



________________________________________________

## Expressions, Statements, and Blocks

## Expressions

An expression is a construct made up of variables, operators, and method invocations, which are constructed according to the syntax of the language, that evaluates to a single value

The Java programming language allows you to construct compound expressions from various smaller expressions as long as the data type required by one part of the expression matches the data type of the other.


## Statements

 A statement forms a complete unit of execution.  Expressions can be made into a statement by terminating the expression with a semicolon (;).

types of statements:

 1. expression statements
  example, 
- Assignment expressions
- Any use of ++ or --
- Method invocations
- Object creation expressions

2. declaration statements
3. control flow statements




## Blocks

A block is a group of zero or more statements between balanced braces and can be used anywhere a single statement is allowed. 


_________________________________________

## Control Flow Statements

it breaks up the flow of execution by employing decision making, looping, and branching, enabling your program to conditionally execute particular blocks of code. This section describes the decision-making statements (if-then, if-then-else, switch), the looping statements (for, while, do-while), and the branching statements (break, continue, return) supported by the Java programming language.




___________________________________________________


 ## compile a code

 converting the code into a language that the computer understands 