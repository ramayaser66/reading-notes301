> # Domain modeling 
 A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain.   An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

## Define a constructor and initialize properties
var nameA = function (param1, param2){
this.propertyName =  a description of the property; 
}
Var name = new nameA(parama, paramb); 	
When the function is called, the data inside these parameters are stored inside the properties respectively. Storing data within properties ensures any newly created object can access that data later.
After the constructor function definition, two objects are instantiated with the new keyword and their properties are initialized by calling the constructor function.  After being instantiated and initialized, these objects are stored inside the variables. 
### Object-oriented programming in JavaScript 
-	The new keyword instantiates (i.e. creates) an object.
-	 The constructor function initializes properties inside that object using the this variable. 
-	The object is stored in a variable for later use.

## Generate random numbers
-	 Random number generator ( Math.random()) 
Object name.property. generateRandom = function(min, max) {
  return Math.floor(Math.random() * (max - min + 1)) + min;}


## Summary 
______________________________________________________


Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.


-	When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
-	 Model its attributes with a constructor function that defines and initializes properties.
-	Model its behaviors with small methods that focus on doing one job well.
-	Create instances using the new keyword followed by a call to a constructor function.
-	Store the newly created object in a variable so you can access its properties and methods from outside.
-	Use the this variable within methods so you can access the object's properties and methods from inside.


> # Tables 
Information displayed in a grid made up of rows and columns.

## Basic Table Structure
-	The table element, is used to create a table. The contents of the table are written out row by row. 
-	The tr tag, You indicate the start of each row using the opening tr tag. (The tr stands for table row.) It is followed by one or more td elements (one for each cell in that row).At the end of the row you use a closing tr tag. 

-	The td tag,  Each cell of a table is represented using a td element. (The td stands for table data.) At the end of each cell you use a closing td tag 

## Table Headings 
-	The th tag, t is used just like the td element but its purpose is to represent the heading for either a column or a row. (The th stands for table heading.)
-	 Even if a cell has no content, you should still use a td or th element to represent the presence of an empty cell otherwise the table will not render correctly. (The first cell in the first row of this example shows an empty cell.)
-	You can use the scope attribute on the th element to indicate whether it is a heading for a column or a row. It can take the values: row to indicate a heading for a row or col to indicate a heading for a column.




## Spanning Columns/ rows 
The entries in a table to stretch across more than one column or down across more than one row.
-	The colspan attribute can be used on th or td  element and indicates how many columns that cell should run across.
-	The rowspan attribute can be used on a th or td  element to indicate how many rows a cell should span down the table.


 ## Long TABLES 

There are three elements that help distinguish between the main content of the table and the first and last rows (which can contain different content).
-	Thead 
The headings of the table should sit inside the thead element.
-	Tbody
The body should sit inside the tbody element.
-	Tfoot
The footer belongs inside the tfoot element.


## Old Code: Width & Spacing

-	The width attribute 

was used on the opening table tag to indicate how wide that table should be and on some opening th and td tags to specify the width of individual cells.  The value of this attribute is the width of the table or cell in pixels.



-	The opening table tag 

 could also use the cellpadding attribute to add space inside each cell of the table, and the cellspacing attribute to create space between each cell of the table. The values for these attributes were given in pixels. 



> # functions, methods and objects 

## creating an object: constructor notation 
 

-	First, you create a new object using a combination of the new keyword and the object() constructor function. 
Var Name = new object(); 

You can use this syntax to add properties and method to any object you have created 

## Updating an object 
-	Object.propertyname = ‘property value’; 
-	Object[‘propertyname’] = ‘property value’;

Use a dot notation or square brackets. They work on objects created using literal or constructor notation. 
To delete a property, use the delete keyword. 
## this keyword 
____________________________________________________

The keyword is used inside functions and objects.
-	A FUNCTION IN GLOBAL SCOPE 
When a function is created at the top level of a script (that is, not inside another object or function), then it is in the global scope or global context.
-	GLOBAL VARIABLES
 All global variables also become properties of the object. So when a function is in the global context, you can access global variables using the object, as well as its other properties.
-	A METHOD OF AN OBJECT 
When a function is defined inside an object, it becomes a method. In a method, this refers to the containing object.
-	FUNCTION EXPRESSION AS METHOD 
If a named function has been defined in global scope, and it is then used as a method of an object, this refers to the object it is contained within.


## Objects 
_________________________________________________
<br>

If you want to access items via a property name or key, use an object (but note that each key in the object must be unique). If the order of the items is important, use an array.

-	INDIVIDUAL OBJECTS
 Objects store sets of name/value pairs. They can be properties (variables) or methods (functions). The order of them is not important (unlike the array). You access each piece of data by its key. In object literal notation, properties and methods of an object are given in curly braces {}
Var object name = {
Key1:  ‘property one value’, 
Key2:  ‘property two value’, }
-	MULTIPLE OBJECTS
 When you need to create multiple objects within the same page, you should use an object constructor to provide a template for the objects.
  
  





 








  
  





 







