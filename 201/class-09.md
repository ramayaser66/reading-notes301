> # Forms 
A group of elements put together that allow you to take information from users to your site.

## Form Controls 


### Adding Text 
-	Text input (single-line) 
-	Password input 
-	Text area (multi-line)

### Making Choices 
-	Radio buttons
-	Checkboxes
-	Drop-down boxes
### Submitting Forms 
-	Submit buttons
-	Image buttons 


### Uploading Files 
-	File upload


Note: A form may have several form controls, each gathering different information. The server needs to know which piece of inputted data corresponds with which form element.

## Form Structure 
-	The form tag 
-	Form attribute
Action : 
 Every form element requires an action attribute. Its value is the URL for the page on the server that will receive the information in the form when it is submitted. 
Method: 
Forms can be sent using one of two methods: get or post.
-	With the get method, the values from the form are added to the end of the URL specified in the action attribute. The get method is ideal for:
1.	short forms (such as search boxes)
2.	when you retrieve  data from a web server

-	With the post method the values are sent in what are known as HTTP headers. As a rule of thumb you should use the post method if your form:
1.	allows users to upload a file
2.	is very long
3.	contains sensitive data (e.g. passwords)
4.	adds information to, or deletes information from, a database

## Text Input 
The Input element is used to create several different form controls. The value of the type attribute determines what kind of input they will be creating.
( type=”test”)
It creates a single line input 
(name)
To know which form control each piece of data was entered into.
(size)
Note:
The size attribute should not be used on new forms
It was used in older forms to indicate the width of the text input

(Maxlength)
 You can use the maxlength attribute to limit the number of characters a user may enter into the text field. Its value is the number of characters they may enter.

Notes:
- Whenever you want to collect information from visitors you will need a form, which lives inside a form element.
 - Information from a form is sent in name/value pairs.
 -  Each form control is given a name, and the text the user types in or the values of the options they select are sent to the server. 
- HTML5 introduces new form elements which make it easier for visitors to fill in forms.



# LISTS, TABLES AND FORMS
## Bullet point styles 
List-style-type 
The list-style-type property allows you to control the shape or style of a bullet point
It is used in:

-	ordered lists 
1.	decimal
2.	decimal-loading-zero
3.	lower-alpha
4.	lower-roman 
5.	upper-roman

-	unordered list
-	lists 

 ## Images for bullets 
Life-style-image 
You can specify an image to act as a bullet point using the list-style-image property.

## positioning the Marker
List-style-position 
Lists are indented into the page by default and the list-styleposition property indicates whether the marker should appear on the inside or the outside of the box containing the main points.
This property can take one of two values:
-	outside
The marker sits to the left of the block of text.
-	Inside
The marker sits inside the box of text 

## List shorthand 
List-style 
As with several of the other CSS properties, there is a property that acts as a shorthand for list styles. It is called list-style, and it allows you to express the markers' style, image and position properties in any order 

# Table Properties 
You have already met several properties:
-	Width 
-	Padding 
-	Text-transform 
-	Lette-spaceing.font size 
-	Border-top. border-bottom 
-	Text-align 
-	Background-color 
-	:hover 
## staylling tables:
-	Give cells padding
-	Distinguish headings
-	Shade alternate rows
-	Align numerals

##  border on Empty Cells
Empty-cells
If you have empty cells in your table, then you can use the empty-cells property to specify whether or not their borders should be shown.

-	Show
-	Hide
-	Inherit 

 ## Gaps Between cells
 Border-spacing, border-collapse 
The border-spacing property allows you to control the distance between adjacent cells. By default, browsers often leave a small gap between each table cell, so if you want to increase or decrease this space then the border-spacing property allows you to control the gap. 
-	Collapse
-	Separate

Notes:
-	In addition to the CSS properties covered in other chapters which work with the contents of all elements, there are several others that are specifically used to control the appearance of lists, tables, and forms.
-	 List markers can be given different appearances using the list-style-type and list-style image properties.
-	Table cells can have different borders and spacing in different browsers, but there are properties you can use to control them and make them more consistent.
-	Forms are easier to use if the form controls are vertically aligned using CSS.
-	Forms benefit from styles that make them feel more interactive.



# Events 
## Different Events Type
1.	UI events 
-	Load: Web page has finished loading
-	Unload: Web page is unloading (usually because a new page was requested)
-	Error: Browser encounters a JavaScript error or an asset doesn't exist
-	Resize: Browser window has been resized
-	Scroll: User has scrolled up or down the page 

2.	KEYBOARD EVENTS
-	Keydown: User first presses a key (repeats while key is depressed)
-	Keyup: User releases a key
-	Keypress: Character is being inserted (repeats while key is depressed) 

3.	MOUSE EVENTS

-	Click
-	dbl click
-	moused own
-	mouseup
-	mousemove
-	mouseout

And many others



Summary 

-	Events are the browser's way of indicating when something has happened (such as when a page has finished loading or a button has been clicked).
-	 Binding is the process of stating which event you are waiting to happen, and which element you are waiting for that event to happen upon.
-	 When an event occurs on an element, it can trigger a JavaScript function. When this function then changes the web page in some way, it feels interactive because it has responded to the user.
-	 You can use event delegation to monitor for events that happen on all of the children of an element. 
-	The most commonly used events are W3C DOM events, although there are others in the HTMLS specification as well as browser-specific events.




