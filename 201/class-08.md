> # Layout 

![layout](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTbyiqbzEEvkZhwBTzNAe1dLXec8agcgkZrHg&usqp=CAU) 


The design of evryelement on your page and how to make your page more attractive and easy on the eyes! 

## positioning elements 
1.	Building Blocks 
To css every Html element is locateded inside a box ## [ margin, border, padding and content] 
-	Block level box ## [example: h1-h6,   p,   ul,  li] 
Block-level boxes start on a new line and act as the main building blocks of any layout,
-	Inline box  ## [ img,  b, I ] 
e inline boxes flow between surrounding text. You can control how much space each box takes up by setting the width and height of the boxes

##  Containing Elements 
Note: If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.
-	A box may be nested inside several other block-level elements. The containing element is always the direct parent of that element. 

##  Controlling the Position of Elements 
positioning schemes, that allow you to control the layout of a page:
-	Normal flow 
Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one.  For example: the paragraphs appear one after the other, vertically down the page.
( position:static)
As mentioned earlier, in normal flow, each block-level element sits on top of the next one.
It is the browser default way in positioning the elements. 
Is Css you can assignee position: static 
For example in the h1 element you don’t have to assignee a width property and you can see it stretch by default. 

-	Relative Positioning 
This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed. 
You can indicate that an element should be relatively positioned using the position property with a value of relative.
(position:relative)

-	Absolute positioning 
This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position of any surrounding elements (as they simply ignore the space it would have taken up) 
(position:absolute)


### Box offset 
Box offset properties, how far from the top or bottom and left or right the element  should be placed
-	Fixed Positioning 
This is a form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element.
(position:fixed) 
It positions the element in relation to the browser window. Therefore, when a user scrolls down the page, it stays in the exact same place.
To control where the fixed position box appears in relation to the browser window, the box offset properties are used.

-	Floating Elements 
Floating an element allows you to take that element out of normal flow and position it to the far left or right of a containing box. The floated element becomes a block-level element around which other content can flow. 
(float)
When you use the float property, you should also use the width property to indicate how wide the floated element should be.
###  using Float to Place Elements Side-by-Side
Note: When elements are floated, the height of the boxes can affect where the following elements sit.
-	Clearing floats 
(clear)
The clear property allows you to say that no element (within the same containing element) should touch the left or right hand sides of a box. It can take the following values: 
-	Left
The left-hand side of the box should not touch any other elements appearing in the same containing element 

-	right 
The right-hand side of the box will not touch elements appearing in the same containing element.
-	Both 
Neither the left nor right-hand sides of the box will touch elements appearing in the same containing element. 
-	None 
Elements can touch either side.


## NOTES TO REMEMBER 
-	 elements are often used as containing elements to group together sections of a page.
-	Browsers display pages in normal flow unless you specify relative, absolute, or fixed positioning. 
-	The float property moves content to the left or right of the page and can be used to create multi-column layouts. (Floated items require a defined width.)
-	 Pages can be fixed width or liquid (stretchy) layouts.
-	 Designers keep pages within 960-1000 pixels wide, and indicate what the site is about within the top 600 pixels (to demonstrate its relevance without scrolling).
-	Grids help create professional and flexible designs. 
-	CSS Frameworks provide rules for common tasks. X You can include multiple CSS files in one page
