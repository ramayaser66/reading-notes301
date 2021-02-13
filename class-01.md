# Responsive Web Design

![rwd]( https://s8m9g4v9.rocketcdn.me/wp-content/uploads/2014/06/responsive-webdesign.jpg)

People today tend to use mobile phones and mobile devices over their computers and desktops which created the need for the responsive web design. 
 
-	Responsive overview 
Building a website that is able to work on every device and every screen size, no matter how large or small, mobile or desktop is known as RWD.
It is focused around giving the user an intuitive and gratifying experience whether it’s a desktop computer or a cell phone user. They all benefit from responsive websites.
-	Responsive vs. Adaptive vs. Mobile

The difference between all of them: 
Responsive and adaptive web design are almost the same. 
Responsive: means to react quickly and positively to any change. Websites continually and fluidly change based on different factors, such as viewport width.

Adaptive:  to be easily modified for a new purpose or situation. Adaptive websites are built to a group of preset factors. A combination of the two is ideal, providing the perfect formula for functional websites. 

Mobile:  to build a separate website commonly on a new domain solely for mobile users. Mobile websites can be extremely light but they do come with the dependencies of a new code base and browser sniffing. 

## Responsive web design is broken down into three main components:


1.	Flexible Layouts
 The practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width. Flexible grids are built using relative length units, most commonly percentages or em units.
 These relative lengths are then used to declare common grid property values such as: 
-width. 
-margin.
- padding.
## Note: Flexible layouts do not advocate the use of fixed measurement units, such as pixels or inches. 

2.	media queries
Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation. There are a couple different ways to use media queries:
-	Using the @media rule inside of an existing style sheet. 
-	Importing a new style sheet using the @import rule. 
-	Linking to a separate style sheet from within the HTML document.
## Note: Each media query may include a media type followed by one or more expressions. Common media types include all, screen, print, tv, and braille. 
Media Features in Media Queries: 
Media features identify what attributes or properties will be targeted within the media query expression. 
Height & Width Media Features: 
The height and width features are based off the height and width of the viewport rendering area, the browser window for example. Values for these height and width media features may be any length unit, relative or absolute.

Orientation Media Feature: 
The orientation media feature determines if a device is in the landscape or portrait orientation.
-	landscape mode, is triggered when the display is wider than taller.
-	portrait mode , is triggered when the display is taller than wider. 

Aspect Ratio Media Features:
The aspect-ratio and device-aspect-ratio features specifies the width/height pixel ratio of the targeted rendering area or output device.
The value for the aspect ratio feature consist of two positive integers separated by a forward slash. The first integer identifies the width in pixels while the second integer identifies the height in pixels.


 Resolution Media Feature: 

specifies the resolution of the output device in pixel density, also known as dots per inch or DPI.  Does accept the min and max prefixes. Additionally, the resolution media feature will accept dots per pixel (1.3dppx), dots per centimeter (118dpcm), and other length based resolution values. 

Viewport
-	Viewport Height & Width: 
The viewport Meta tag with either the height or width values will define the height or width of the viewport respectively. 
For the height property the keyword device-height value is accepted, and for the width property the keyword device-width is accepted. Using these keywords will inherit the device’s default height and width value. 

-	Viewport Scale: 
Control how a website is scaled on a mobile device, and how users can continue to scale a website, use the minimum-scale, maximum-scale, initial-scale, and user-scalable properties. 




3.	flexible media

 As viewports begin to change size media doesn’t always follow suit. Images, videos, and other media types need to be scalable, changing their size as the size of the viewport changes. 
Using the max-width property with a value of 100%. Doing so ensures that as the viewport gets smaller any media will scale down according to its containers width. 

-	Flexible Embedded Media:
 
The max-width property doesn’t work well for all instances of media, specifically around iframes and embedded media. When it comes to third party websites, 
To get embedded media to be fully responsive, the embedded element needs to be absolutely positioned within a parent element. The parent element needs to have a width of 100% so that it may scale based on the width of the viewport. The parent element also needs to have a height of 0 to trigger the hasLayout mechanism within Internet Explorer. 
Padding is then given to the bottom of the parent element, the value of which is set in the same aspect ratio of the video. This allows the height of the parent element to be proportionate to that of it’s width.



># Float 

![float]( https://csspark.com/wp-content/uploads/2014/09/web-layout.png)

Float is a CSS positioning property. 
-	print layout,
 images may be set into the page such that text wraps around them as needed. This is commonly and appropriately called “text wrap”. 
the boxes that hold the text can be told to honor the text wrap, or to ignore it. Ignoring the text wrap will allow the words to flow right over the image like it wasn’t even there. This is the difference between that image being part of the flow of the page (or not). 

-	web design, 
page elements with the CSS float property applied to them are just like the images in the print layout where the text flows around them. Floated elements remain a part of the flow of the web page. This is distinctly different than page elements that use absolute positioning. 


Absolutely positioned page elements are removed from the flow of the webpage, like when the text box in the print layout was told to ignore the page wrap. Absolutely positioned page elements will not affect the position of other elements and other elements will not affect them, whether they touch each other or not. 



### There are four valid values for the float property:

- Left  float
- Right float
- None 
-  Inherit 


floats can be used to create entire web layouts. 



### Clearing the Float
 The clear property:
 An element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float. 

Clear has four valid values:

-	both 
-	left
-	right
-	none 

### The Great Collapse 

Collapsing almost always needs to be dealt with to prevent strange layout and cross-browser problems. We fix it by clearing the float after the floated elements in the container but before the close of the container. 

### Techniques for Clearing Floats

-	The Empty Div Method 
-	The Overflow Method 
-	The Easy Clearing Method 


### Problems with Floats
-	Pushdown  
-	Double Margin Bug
-	3px Jog 
-	Bottom Margin Bug 














