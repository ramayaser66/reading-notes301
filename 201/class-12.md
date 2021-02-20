# Charts 
![charts](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR0g0iL8rdgNeA_TJWMqqsxTgnLUEHr6M7y5g&usqp=CAU)

Charts are better for displaying data visually than tables. They’re easier to look at and convey data quickly, but they’re not always easy to create.


## Types of charts 


-	bar charts, 
-	line charts, 
-	charts


## Dealing with charts in JavaScript

a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well-documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.

## How to use charts.js 

-	setting up 
-	drawing a line chart 
-	Drawing a  chart 



##  drawing a line chart
1.	The first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart. 
2.	 write a script that will retrieve the context of the canvas
3.	Inside the same script tags we need to create our data. Labels for the base of our chart and datasets to describe the values on the chart.



## drawing a pie chart
1.	We need the canves element and we need to get the context and to instantiate the chart.

2.	supply some options to the chart.

3.	 create the data. This data is a little different to the line chart because the pie chart is simpler, we just need to supply a value and a color for each section. 

4.	 add  options

-	remove the stroke from the segments. 
-	animate the scale of the pie so that it zooms out from nothing.


## drawing a bar chart 

the syntax for the bar chart is very similar to the line chart
1.	add the canvas element
2.	retrieve the element and create the graph
3.	add in the bar chart’s data


Notes: The great things about Chart.js are that it’s simple to use and really very flexible. Plus, once you’ve mastered the basics here, you’ll discover that there are tons of options




# basic usage of canvas

![canvas](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQrDkc6eVRlIbROYZ6KBQZcE4EeA6jI25D2bg&usqp=CAU)


canvas and img tags are similar but with a key difference that is canvas doesn’t have src and alt attributes. 

Canvas has only two attributes 
-	width 
-	height 
they are optional and can be set using DOM properties 

if they are not specified, canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size


 # using the id attribute 
Id can be applied to any HTML element. it makes it a lot  easier to identify it in a script.
The canvas element can be styled just like any normal image.
These rules, however, don't affect the actual drawing on the canvas. When no styling rules are applied to the canvas it will initially be fully transparent.

## fallback content 
![fallback](https://i.ytimg.com/vi/0eV6yL162Kw/mqdefault.jpg)


The canvas element differs from other elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers.

-  Providing fallback content  
insert the alternate content inside the canvas element. Browsers that don't support canvas will ignore the container and render the fallback content inside it. Browsers that do support it will ignore the content inside the container, and just render the canvas normally.

-	Required canvas closing tag 
The closing tag (</canvas>) is required. If this closing tag is not present, the rest of the document would be considered the fallback content and wouldn't be displayed.

## The rendering context 

The canvas is initially blank. To display something, a script first needs to access the rendering context and draw on it. The <canvas> element has a method called getContext(), used to obtain the rendering context and its drawing functions. getContext() takes one parameter, the type of context.






# drawing shapes with canvas 


## The Gird (coordinate space.)


canvas has a default grid overlayed.
Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at coordinate (0,0). All elements are placed relative to this origin. So the position of the top left corner of the blue square becomes x pixels from the left and y pixels from the top, at coordinate (x,y)


## drawing rectangles 

Canvas only supports two primitive shapes. All other shapes must be created by combining one or more paths. 

Canvas shapes:


-  rectangles
There are three functions to draw rectangles 
1.	fillRect(x, y, width, height), Draws a filled rectangle.
2.	strokeRect(x, y, width, height), Draws a rectangular outline.
3.	clearRect(x, y, width, height), Clears the specified rectangular area, making it fully transparent.

-  paths (lists of points connected by lines)

A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color

1.	create the path.
2.	Then you use drawing commands to draw into the path.
3.	Once the path has been created, you can stroke or fill the path to render it.


 functions used to perform these steps:
-	beginPath() 
Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
-	Path methods 
Methods to set different paths for objects.
-	closePath()
Adds a straight line to the path, going to the start of the current sub-path.

-	closePath()
Adds a straight line to the path, going to the start of the current sub-path
-	stroke()
Draws the shape by stroking its outline.
-	fill()
Draws a solid shape by filling the path's content area.



# Applying styles and colors

## colors 
a string representing a CSS <color>, a gradient object, or a pattern object. We'll look at gradient and pattern objects later. By default, the stroke and fill color are set to black (CSS color value #000000).

to apply colors to a shape, there are two important properties we can use:
-	fillStyle = color
Sets the style used when filling shapes.
-	strokeStyle = color
Sets the style for shapes' outlines.

##  line style 

roperties which allow us to style lines:

-	neWidth = value
Sets the width of lines drawn in the future.
-	lineCap = type
Sets the appearance of the ends of lines.
-	lineJoin = type
Sets the appearance of the "corners" where lines meet.
-	miterLimit = value
Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.
-	getLineDash()
Returns the current line dash pattern array containing an even number of non-negative numbers.
-	setLineDash(segments)
Sets the current line dash pattern.
-	lineDashOffset = value
Specifies where to start a dash array on a line.
	


## Gradients

 Fill and stroke shapes using linear and radial gradients. We create a CanvasGradient object by using one of the following methods. We can then assign this object to the fillStyle or strokeStyle properties.
-	createLinearGradient(x1, y1, x2, y2)
Creates a linear gradient object with a starting point of (x1, y1) and an end point of (x2, y2).
-	createRadialGradient(x1, y1, r1, x2, y2, r2)
Creates a radial gradient. The parameters represent two circles, one with its center at (x1, y1) and a radius of r1, and the other with its center at (x2, y2) with a radius of r2.


## shadows 
Using shadows involves just four properties:

-	shadowOffsetX = float
Indicates the horizontal distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.
-	shadowOffsetY = float
Indicates the vertical distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.
-	shadowBlur = float
Indicates the size of the blurring effect; this value doesn't correspond to a number of pixels and is not affected by the current transformation matrix. The default value is 0.
-	shadowColor = color
A standard CSS color value indicating the color of the shadow effect; by default, it is fully-transparent black.
The properties shadowOffsetX and shadowOffsetY indicate how far the shadow should extend from the object in the X and Y directions; these values aren't affected by the current transformation matrix. Use negative values to cause the shadow to extend up or to the left, and positive values to cause the shadow to extend down or to the right. These are both 0 by default.
The shadowBlur property indicates the size of the blurring effect; this value doesn't correspond to a number of pixels and is not affected by the current transformation matrix. The default value is 0.

 















 



