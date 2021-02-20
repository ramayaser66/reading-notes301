 
>  # Images
___________________________________________________________________

A picture makes the difference between an average-looking site and a really engaging one! 

## Storing Images on Your Site:
![images](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQCGeZGIiNTbbnNU2Z-sEM1daKXr6zH7EFhuA&usqp=CAU)

Note: If you are building a site from scratch, it is good practice to create a folder for all of the images the site uses.

## Adding Images 
To add an image into the page you need to use an “ <img>” element This is an empty element (which means there is no closing tag). It must carry the following two attributes:
-	Src 
This tells the browser where it can find the image file. This will usually be a relative URL pointing to an image on your own site.
-	alt 
This provides a text description of the image which describes the image if you cannot see it. 
The text used in the alt attribute is often referred to as alt text. It should give an accurate description of the image content so it can be understood by screen reader software (used by people with visual impairments) and search engines. 

-	title
You can also use the title attribute with the Error! Filename not specified.element to provide additional information about the image. Most browsers will display the content of this attribute in a tootip when the user hovers over the image. 

## Height & Width of Images 
You will use “<img>” tag with: 
-	height 
This specifies the height of the image in pixels. 

-	width 
 This specifies the width of the image in pixels 

## Aligning Images Horizontally 
The align attribute can take these horizontal values:
-	left 
 This aligns the image to the left (allowing text to flow around its right-hand side).
-	Right 
This aligns the image to the right (allowing text to flow around its left-hand side).

## Aligning Images Vertically 
-	Top 
This aligns the first line of the surrounding text with the top of the image. 
-	Middle
This aligns the first line of the surrounding text with the middle of the image 
-	Bottom 
This aligns the first line of the surrounding text with the bottom of the image. 

##  Image Resolution
Images created for the web should be saved at a resolution of 72 ppi. The higher the resolution of the image, the larger the size of the file. 

________________________________________________________________________________________________________________________________

> # Color!

![color](https://miro.medium.com/max/1680/1*ECJO0bO2oHJwm-wlrbr7Ag.png)

Note: Every color on a computer screen is created by mixing amounts of red, green, and blue. 
.

The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:
-	rgb values
These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90) 
-	hex codes

These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: #ee3e80
-	color names 
There are 147 predefined color names that are recognized by browsers. For example: DarkCyan 
## Background Color ( background-color)

CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box. You can specify your choice of background color in the same three ways you can specify foreground colors: RGB values, hex codes, and color names (covered on the next page). If you do not specify a background color, then the background is transparent 

### finding the right color 
To find the color you want, you can use a color picker 
-	Color picking tools are available in image editing programs like Photoshop and GIMP. You can see the RGB values specified next to the radio buttons that say R, G, B. 

## Contrast 
When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible. 

##  Opacity (opacity, rgba) 
CSS3 introduces the opacity property which allows you to specify the opacity of an element and any of its child elements. The value is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity). 
The CSS3 rgba property allows you to specify a color, just like you would with an RGB value, but adds a fourth value to indicate opacity. This value is known as an alpha value 

Note: CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA. 
___________________________________________________________________________________________________________________________________________________________

> # Text 

![text](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT1tAewI46AuEQLDq8uEyj6hG5J01Ly3um5pg&usqp=CAU)


-	Serif 
Serif fonts have extra details on the ends of the main strokes of the letters. These details are known as serifs.
-	Sans-Serif 
 Sans-serif fonts have straight ends to letters, and therefore have a much cleaner design. 
-	Monospace 
Every letter in a monospace (or fixed-width) font is the same width. (Non-monospace fonts have different widths.) 

###  weight:
-	Light 
-	Medium 
-	Bold 
-	Black 
###  style 
-	Normal
-	Italic 
-	Oblique

### stretch:
-	Condensed 
-	Regular
-	Extended 

Notes: 
-	X You can control the space between lines of text, individual letters, and words. Text can also be aligned to the left, right, center, or justified. It can also be indented. 

-	You can use pseudo-classes to change the style of an element when a user hovers over or clicks on text, or when they have visited a link. 

