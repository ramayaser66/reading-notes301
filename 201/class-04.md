
# Read-04
> # LINKS 

Allow you to move from one web page to another — enabling the very idea of browsing or surfing.

 types of links:
	 
	- Links from one website to another. 
	  
	- Links from one page to another on the same website. 
	 
	- Links from one part of a web page to another part of the same page. 
	 
	- Links that open in a new browser window. 

	-Links that start up your email program and address a new email to someone.
    


Links are created using the (a)  element. Users can click on anything between the opening  (a) tag and the closing  (a) tag. You specify which page you want to link to using the href attribute.


-	Linking to Other Sites: 

Links are created using the (a) element which has an attribute called href.
 The value of the href attribute is the page that you want people to go to when they click on the link. 
Users can click on anything that appears between the opening tag and the closing tag and will be taken to the page specified in the href attribute. When you link to a different website, the value of the href attribute will be the full web address for the site, which is known as an absolute URL.

-	Linking to Other Pages on the Same Site:

When you are linking to other pages within the same site, you do not need to specify the domain name in the URL. You can use a shorthand known as a relative URL.
If all the pages of the site are in the same folder, then the value of the href attribute is just the name of the file. 
_____________________________________________

##  Directory Structure
On larger websites it's a good idea to organize your code by placing the pages for each different section of the site into a new folder. Folders on a website are sometimes referred to as directories. 




## Relative URLs 

When you are linking to a page on your own website, you do not need to specify the domain name. You can use relative URLs which are a shorthand way to tell the browser where a page is in relation to the current page.

### Note:
 If all of the files in your site are in one folder, you simply use the file name for that page. If your site is organized into separate folders (or directories), you need to tell the browser how to get from the page it is currently on to the page that you are linking to.


##  Email Links 

To create a link that starts up the user's email program and addresses an email to a specified email address, you use the (a) element. However, this time the value of the href attribute starts with mailto: and is followed by the email address you want the email to be sent to.


-	Opening Links in a New Window using  (target attribute) on the opening tag.

-	Linking to a Specific Part of the Same Page, identify the points in the page that the link will go to. You do this using the id attribute . To link to an element that uses an id attribute you use the (a) element again, but the value of the href attribute starts with the # symbol, followed by the value of the id attribute of the element you want to link to.

-	Linking to a Specific Part of Another Page, Therefore, the href attribute will contain the address for the page (either an absolute URL or a relative URL), followed by the # symbol, followed by the value of the id attribute that is used on the element you are linking to.

> #  Layout 

## Building Blocks

CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.
You can control how much space each box takes up by setting the width of the boxes (and sometimes the height, too). To separate boxes, you can use borders, margins, padding, and background colors 

## Containing Elements 
If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element. 
Note: you might group together all of the elements that form the header of a site (such as the logo and the main navigation). The 
element that contains this group of elements is then referred to as the containing element.

## Controlling the Position of Elements 
- Normal flow
The paragraphs appear one after the other, vertically down the page
- Relative Positioning 
The second paragraph has been pushed down and right from where it would otherwise have been in normal flow.
- Absolute positioning
The heading is positioned to the top right, and the paragraphs start at the top of the screen (as if the heading were not there).

## Box offset properties:
Tell the browser how far from the top or bottom and left or right it should be placed 
- Fixed Positioning
The heading has been placed in the center of the page and 25% from the top of the screen. (The rest appears in normal flow.)
- Floating Elements
The heading has been floated to the left, allowing the paragraphs of text to flow around It 


## Normal Flow
 In normal flow, each block-level element sits on top of the next one. Since this is the default way in which browsers treat HTML elements, you do not need a CSS property to indicate that elements should appear in normal flow, but the syntax would be: position: static;
## Relative Positioning
 position:relative 
Relative positioning moves an element in relation to where it would have been in normal flow. 

## Absolute Positioning
position:absolute 
When the position property is given a value of absolute, the box is taken out of normal flow and no longer affects the position of other elements on the page. (They act like it is not there.) 

## Fixed Positioning
 position:fixed
Fixed positioning is a type of absolute positioning that requires the position property to have a value of fixed. It positions the element in relation to the browser window. 

##  Fixed Width Layouts
Fixed width layout designs do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels 

 
>  # functions, Methods and Objects 

 ## Functions &methods 
-	Functions consist of a series of statements that have been grouped together because they perform a specific task. A method is the same as a function, except methods are created inside (and are part of) an object.

Step one: Declaring a function 

Step two: Calling a function 



## Objects 
-	objects are made up of properties and methods. 
-	 BUILT-IN METHODS OBJECTS, The browser comes with a set of objects that act like a toolkit for creating interactive web pages. 
 
##  MEMORY & VARIABLES
Global variables use more memory. The browser has to remember them for as long as the web page using them is loaded. Local variables are only remembered during the period of time that a function is being executed.
## pair programming 
-  Greater efficiency
 - Engaged collaboration
- Learning from fellow students
- Work environment readiness
- Social skills- Job interview readiness



