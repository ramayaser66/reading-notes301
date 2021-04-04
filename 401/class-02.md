# Packages and Import 

![](https://media.geeksforgeeks.org/wp-content/uploads/java-types-of-packages.jpg)

a package is the directory that contains the Java files. 
 one declares the packages when  defying  Java program,  name the packages needed  from other libraries and import them


 ## Package declaration 

using import statements,
which allow you to specify classes from other packages that can be referenced without qualifying them with their package.

Java creates what it calls a default package.
-  it's possible to omit the package declaration.


## Package declaration syntax
- Package statment (optional).
- Imports (optional).
- Class or interface definitions.


import java.awt.*;

public class Drawing {
    . . .
}



## Imports: three options

import javax.swing.*;  // Make all classes visible altho only one is used.

class ImportTest {
    public static void main(String[] args) {
        JOptionPane.showMessageDialog(null, "Hi");
        System.exit(0);
    }
}



## Common imports


import java.awt.*;	Common GUI elements.
import java.awt.event.*;	The most common GUI event listeners.
import javax.swing.*;	More common GUI elements. Note "javax".
import java.util.*;	Data structures (Collections), time, Scanner, etc classes.
import java.io.*;	Input-output classes.
import java.text.*;	Some formatting classes.
import java.util.regex.*;	Regular expression classes.

_______________________________________________


# Java loops

![](https://appdividend.com/wp-content/uploads/2019/07/Java-For-Loop-Example-For-Loop-in-Java-Tutorial.png)

a loop is a a control flow statement that executes a part of the programs repeatedly on the basis of given boolean condition.

 types of loops:
 -  for loops

 it allows to repeat certain operations by incrementing and evaluating a loop counter.

 - Enhanced for-each loop

 - While loop

 - Do-While loop
 the first condition evaluation happens after the first iteration of the loop.

