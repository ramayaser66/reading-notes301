# Error Handling & Debugging 


![error](https://thedataist.com/wp-content/uploads/2016/10/debugging.jpg); 


____________________________________________________________________________________________________________


When you write a long code you’re going to have some mistake in for sure. No gets it right from the first time. It’s a must. Especially if you are a beginner at the whole programming process!
A good way to know your mistake and solving whatever error you is your browser, it will help you determine it and you will have a way of fixing it. 
## Order of execution 
Following the order of your code & your script and knowing the order it is executed helps you know how it is processed. Some tasks cannot complete until another statement or function has been run.

## EXECUTION CONTEXT
Every statement in a script lives in one of three execution contexts:
-	GLOBAL CONTEXT
Code that is in the script, but not in a function. There is only one global context in any page.
FUNCTION CONTEXT 
Code that is being run within a function. Each function has its own function context.
-	EVAL CONTEXT (NOT SHOWN)
Text is executed like code in an internal function called eva l {)
  VARIABLE SCOPE
The first two execution contexts correspond with the notion of scope

-	GLOBAL SCOPE
If a variable is declared outside a function, it can be used anywhere because it has global scope. If you do not use the var keyword when creating a variable, it is placed in global scope.
FUNCTION-LEVEL SCOPE
When a variable is declared within a function, it can only be used within that function. This is because it has function-level scope

##  EXECUTION CONTEXT & HOISTING
-	Each time a script enters a new execution context, there are two phases of activity:

1.	PREPARE
-	The new scope is created
-	Variables, functions, and arguments are created
-	The value of the this keyword is determined

2.	EXECUTE

-	Now it can assign values to variables
-	Reference functions and run their cod
-	Execute statements 

#  UNDERSTANDING SCOPE
Functions in JavaScript are said to have lexical scope. They are linked to the object they were defined within. So, for each execution context, the scope is the current execution context's variables object, plus the variables object for each parent execution context. 

If a variable is not found in the variables object for the current execution context, it can look in the variables object of the parent execution context. But it is worth knowing that looking further up the stack can affect performance, so ideally you create variables inside the functions that use them.  

## UNDERSTANDING ERRORS
If you are anticipating that something in your code may cause an error, you can use a set of statements to handle the error. This is important because if the error is not handled, the script will just stop processing and the user will not know why. So exception-handling code should inform users when there is a problem.  

## ERROR OBJECTS
-	When an Error object is created, it will contain the following properties:
1.	Name, Type of execution
2.	Message, Description
3.	fil eNumber, Name of the JavaScript file 
4.	lineNumber, Line number of error. 



-	There are seven types of built-in error objects in JavaScript. You'll see them on the next two pages:
1.	Error, Generic error - the other errors are all based upon this error 
2.	Syntax Error, Syntax has not been followed
3.	Reference Error, Tried to reference a variable that is not declared/within scope
4.	Type Error, An unexpected data type that cannot be coerced
5.	Range Error, Numbers not in acceptable range
6.	URI Error, encode URI (). Decode URI(),and similar methods used incorrectly
7.	Eval Error, eva l () function used incorrectly

Note: When there is an error, you can see all of this information in the JavaScript console I Error console of the browser
## how to handle errors 
two things you can do with the errors:
-	DEBUG THE SCRIPT TO FIX ERRORS
If you come across an error while writing a script (or when someone reports a bug), you will need to debug the code, track down the source of the error, and fix it.

-	HANDLE ERRORS GRACEFULLY
1.	Using try 
2.	Using catch 
3.	Throw
4.	Statements 

Note: Sometimes, an error may occur in the script for a reason beyond your control. For example, you might request data from a third party, and their server may not respond. In such cases, it is particularly important to write error-handling code.


## A DEBUGGING WORKFLOW
Eliminating potential causes of an error.

-	Where is the problem 
narrow down the area where the problem seems to be. In a long script, this is especially important.
-	Check how far the script is running
-	Use breakpoints where things are going wrong
What is the problem
-	When you have set breakpoints, you can see if the variables around them have the values you would expect them to. If not, look earlier in the script 
-	Break down I break out parts of the code to test smaller pieces of the functionality.  
-	Check the number of parameters for a function, or the number of items in an array.  

## Notes:
-	If you understand execution contexts (which have two stages) and stacks, you are more likely to find the error in your code.
-	 Debugging is the process of finding errors. It involves a process of deduction. 
-	The console helps narrow down the area in which the error is located, so you can try to find the exact error.
-	 JavaScript has 7 different types of errors. Each creates its own error object, which can tell you its line number and gives a description of the error. 
-	If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements. Use them to give your users helpful feedback.  






 

