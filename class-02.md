# JQUERY 
![jquery](https://www.tutorialrepublic.com/lib/images/jquery-illustration.png)

An easy and effective way in writing JavaScript codes. 
 the JavaScript file uses the $ () shortcut for the jQuery () function. It selects elements and creates three jQuery objects that hold references to the elements.
-	SIMPLE SELECTORS : 
jQuery uses a language that is already familiar to front-end web developers: CSS selectors. They: 
• Are much faster at selecting elements 
• Can be a lot more accurate about which elements to select
 • Often require a lot less code than older DOM methods
 • Are already used by most front-end developers

### NOTE:  jQuery even adds some extra CSS-style selectors which offer additional 
functionality.

-	COMMON TASKS IN LESS CODE:
jQuery has methods that offer web developers simpler ways to perform common tasks, such as:
 • Loop through elements
 • Add I remove elements from the DOM tree
 • Handle events 
• Fade elements into I out of view
 • Handle Ajax requests

jQuery simplifies each of these tasks, and allows you to write less code to achieve them.


-	CROSS-BROWSER COMPATIBILITY

 jQuery uses feature detection to find the best way to achieve a task. It involves the use of many conditional statements: if the browser supports the ideal way to achieve a task, it us.es that approach; otherwise, it tests to see if it supports the next best option to achieve the same task.


## Finding Elements

- BASIC SELECTORS 
*, All elements.
 Element, All elements with that element name .
#id, Elements whose id attribute has the value specified.
.class, Elements whose cl ass attribute has the value specified.
 Selector1, selector2,  Elements that match more than one selector (see also the .add() method, which is more efficient when combining selections)

-	HIERARCHY
Ancestor descendant, An element that is a descendant of another element. 
Parent > child ,  An element that is a direct child of another element (you can use* in the place of the child to select all child elements of the specified parent). 
Previous + next, Adjacent sibling selector only selects elements that are immediately followed by the previous element. 
 previous – siblings, Sibling selector will select any elements that are a sibling of the previous element. 

-	BASIC FILTERS
: not (selector), All elements except the one in the selector (e.g., div: not ('#summary')).
:first : last , The first element from the selection. 
 :even :od, The last element from the selection. 
:eq(index) , Elements with an even index number in the selection.
:gt(index) , Elements with an odd index number in the selection.
: lt(index) , Elements with an index number equal to the one in the parameter.
 :header, Elements with an index number greater than the parameter. 
:animated, Elements that are currently being animated.
 :focus , The element that currently has focus. 


## ways to include IQUERY in your page 


-	LOADING JQUERY FROM A CDN
-	 EXTENDING JQUERY WITH PLUGINS
-	JAVASCRIPT LIBRARIES
-	JQUERY DOCUMENTATION


jQuery is a JavaScript file you include in your pages. 
Once included, it makes it faster and easier to write cross-browser JavaScript, based on two steps:
1.	Using CSS-style selectors to collect one or more nodes from the DOM tree.
2.	 Using jQuery's built-in methods to work with the elements in that selection.
3.	jQuery's CSS-style selector syntax makes it easier to select elements to work with. It also has methods that make it easier to traverse the DOM. 
4.	jQuery makes it easier to handle events because the event methods work across all browsers.
5.	jQuery offers methods that make it quick and simple to achieve a range of tasks that JavaScript programmers commonly need to perform.

### Type of Events:
    1. Mouse Events
        - click
        - dblclick
        - mouseenter
        - mouseleave
    2. Keyboard Events
        - keyup
        - keydown
        - keypress
    3. Form Events
        - submit
        - change
        - blur
        - focus
    4. Document/Window Events
        - load
        - unload
        - scroll
        - resize


># 6 Reasons for Pair Programming

![h](https://miro.medium.com/max/384/1*KhthCBxD9DhKNkXxSYl9Pw.jpeg)

____________________________________________________

 Pair programming commonly involves two roles: 
-	The Driver. 
Is the programmer who is typing and the only one whose hands are on the keyboard, switching files, version control, and—of course writing code.
-	The Navigators.
Uses their words to guide the Driver but does not provide any direct input to the computer, thinks about the big picture, what comes next, how an algorithm might be converted in to code, he Navigator might also utilize their computer as a second screen to look up solutions and documentation.

Pair programming touches on all four skills: developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves.

## why pair programming?
1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills	
5. Job interview readiness
6. Work environment readiness







