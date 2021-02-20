> # images 

____________________________________________________________________

![images](https://miro.medium.com/max/700/1*rI9vxu3Bv8rNwqMgQ-y_wg.jpeg)



## controlling sizes of images in Css 
You can control the size of an image using:
-	Width
-	Height 

Specifying image sizes helps pages to load more smoothly because the HTML and CSS code will often load before the images, and telling the browser how much space to leave for an image allows it to render the rest of the page without waiting for the image to download.

## aligning images Using Css

Rather than using the img elements align attribute, web page authors are increasingly using the float property to align images. There are two ways that this is commonly achieved:

-	float property 
added to the class that was created to represent the size of the image
-	 New classes
Created with names such as align-left or align-right to align the images to the left or right of the page. These class names are used in addition to classes that indicate the size of the image.

## Centering images Using CSS 
Note: By default, images are inline elements. This means that they flow within the surrounding text 
In order to center an image, it should be turned into a blocklevel element using the display property with a value of block. , there are two common ways in which you can horizontally center an image: 
-	 On the containing element, you can use the text-align property with a value of center 
-	On the image itself, you can use the use the margin property and set the values of the left and right margins to auto.

##  Background Images background-image 

place an image behind any HTML element. This could be the entire page or just part of the page. By default, a background image will repeat to fill the entire box
Background images are often the last thing on the page to load (which can make a website seem slow to load). As with any images you use online, if the size of the file is large it will take longer to download 

##  Repeating Images 
•	background-repeat
•	 background-attachment 

repeat 
background image is repeated both horizontally and vertically

repeat-x 
The image is repeated horizontally only (as shown in the first example on the left) 
repeat-y 
The image is repeated vertically only 
no-repeat 
The image is only shown once 


## Background Position background-position 

This property usually has a pair of values. The first represents the horizontal position and the second represents the vertical. 
-left top
-  left center
-  left bottom
- center top 
- center center 
-center bottom 
-right top 
-right center
- right bottom



> ## practical Information 
______________________________________________________ 

## Search Engine Optimization 

![seo](https://trustlist.uk/wp-content/uploads/2019/07/asa-174.jpg)
-	On-Page 
In every page of your website there are seven key places where keywords (the words people might search on to find your site) can appear in order to improve its findability 
1.	Page Title 
2.	URL / Web Address
3.	Headings
4.	Text
5.	Link Text
6.	Image Alt Text
7.	Page Descriptions


## How to Identify Keywords and Phrases 

identify the right keywords and phrases for your site using :
-	Brainstorm
-	 Organize
-	 Research 
-	Compare
-	Refine
-	Map

## about your Visitors 
-	Signing Up
The Google Analytics service relies on you signing up for an account at: www.google.com/analytics The site will give you a piece of tracking code which you need to put on every page of your site.
-	How it Works
Every time someone loads a page of your site, the tracking code sends data to the Google servers where it is stored. Google then provides a webbased interface that allows you to see how visitors use your site

-	The Tracking Code 
A tracking code is provided by Google Analytics for each website you are tracking. It should appear just before the closing tag. The code does not alter the appearance of your web pages.



## Where Are Your Visitors Coming From? 
-	Referrers 
-	Direct 
-	Search Terms 
-	Advanced Features 



Notes: 

1.	Search engine optimization helps visitors find your sites when using search engines. 
2.	 Analytics tools such as Google Analytics allow you to see how many people visit your site, how they find it, and what they do when they get there.
3.	To put your site on the web, you will need to obtain a domain name and web hosting.
4.	FTP programs allow you to transfer files from your local computer to your web server. 
5.	Many companies provide platforms for blogging, email newsletters, e-commerce and other popular website tools (to save you writing them from scratch).



## Video and Audio APIs


These elements allow us to embed video and audio into web pages.
•	The whole player is wrapped in a (div) element, so it can all be styled as one unit if needed.

•	The (video) element contains two (source) elements so that different formats can be loaded depending on the browser viewing the site.


•	The controls HTML is probably the most interesting

-	We have four buttons 
-	 play/pause, stop, rewind, and fast forward.

Each button has a class name, a data icon attribute for defining what icon should be shown on each button (we'll show how this works in the below section), and an aria label attribute to provide an understandable description of each button, since we're not providing a human-readable label inside the tags. 

The contents of aria label attributes are read out by screen readers when their users focus on the elements that contain them.
There is also a timer div , which will report the elapsed time when the video is playing. Just for fun, we are providing two reporting mechanisms — a span  containing the elapsed time in minutes and seconds, and an extra <div> that we will use to create a horizontal indicator bar that gets longer as the time elapses. 
 
 

 

 