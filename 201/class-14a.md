# what google learned from its quest to build the perfect team 
## Work groups 
<br>

![teamwork](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQLE0Itw5VCqlytVXWggS6noowzOBcTjqwBDw&usqp=CAU)


<br>

Whatever field you in. you are bound to face a situation where you find yourself in a work group.
Work groups differs from one another. And people have different ways of handling and dealing with other people in their work groups. And each prefer a different type of people and different way of dealing with things. Some people prefer strict and ordered group types that have a set of ground rules that they follow and where the work and authority are divided between them. And it is strictly work between them and no side chats or unrelated subjects. 
Others may like the exact opposite were all the work is shared between them without any strict rules or the authority being divided or being in one person’s hand. They all collaborate with brane storming and different ideas in a safe place where no idea is a bad idea. The work has its own time and any extra time left there is room for small talks and getting to know one another so you can feel secure enough around them. 

<br>


> # transforms property

Transform syntax: <br> 
The transform property:  specification of the transform type AKA value (set the specific amount); 

Examples, 

-webkit-transform: scale(1.5);

-moz-transform: scale(1.5);

-transform: scale(1.5);
	
  And so on, 

Properties: 
-	Two dimensional transform property 
 The transform works on the x and y axes, known as horizontal and vertical axes. 
-	Three dimensional transform property 
The transform works on both the x and y axes, as well as the z axis. These three-dimensional transforms help define not only the length and width of an element, but also the depth.


## Two dimensional rotate 
You can rotate an element using different angels with the range of 0o to 360o.
If you set the value to a positive number it will rotate clockwise and if the value is a negative number it would rotate the other way around (counter-clockwise). The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically.

 Code Example, 

.name {
  transform: rotate(20deg);
}






## Two dimensional scale

The transform property has a scale value which you can use to resize your element to the size you want. 
The default size of any element is 1 so if you set the value in the range of (0.1 – 0.99) you element would become smaller than its original size 
But if you set it to a value higher than 1 it would become bigger. 

Code Example, 

 .name {
  transform: scale(.75);
} 


Here it would be smaller than its original size 



.name {
  transform: scale(1.25);

}


Here it would be larger than its original size 



 Ypu can use the scaleX value which will scale the width of an element and the scaleY value which will scale the height of an element



## Two dimensional translate 

Pushing and pulling an element in different directions without interrupting the normal flow of the document. Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis. 
The distance values can be:
-	pixels 
-	Percentages. 

Positive values will push an element down and to the right of its default position while negative values will pull an element up and to the left of its default position. 



## Two dimensional skew 

Is used to distort elements on the horizontal axis, vertical axis, or both.  Using the skewX value distorts an element on the horizontal axis while the skewY value distorts an element on the vertical axis.

Note: The distance calculation of the skew value is measured in units of degrees.
 Length measurements, such as pixels or percentages, do not apply here.


## combining transforms 

Multiple transforms can be combined together. To do it , list the transform values within the transform property one after the other without the use of commas.
Using multiple transform declarations will not work, as each declaration will overwrite the one above it. The behavior in that case would be the same as if you were to set the height of an element numerous times.
 
Code example:
.name {
  transform: skew(10deg, 20deg) translateX(20px);
}



## transform origin 

The default transform origin is the center of an element, both 50% horizontally and 50% vertically. To change this default origin position use the transform-origin property. 
The transform-origin property can accept one or two values. When only one value is specified, that value is used for both the horizontal and vertical axes. If two values are specified, the first is used for the horizontal axis and the second is used for the vertical axis.

 



## three dimensional transforms 
Same as mentioned earlier, the only difference is that I add a value to the z-axis. 
For example with the rotate value:

-	Using the rotateX value allows you to rotate an element around the x axis.
-	Using the rotateY value allows you to rotate an element around the y axis
-	Using the rotateZ value allows an element to be rotated around the z axis.

Positive values will rotate the element around its dedicated axis clockwise, while negative values will rotate the element counterclockwise. 


## backface visibility 
When working with three-dimensional transforms, elements will occasionally be transformed in a way that causes them to face away from the screen. By default these elements are shown from the back. So if you prefer not to see these elements at all, set the backface-visibility property to hidden, and you will hide the element whenever it is facing away from the screen.



# Transitions & Animations
-	 CSS3 transitions 
 the potential to alter the appearance and behavior of an element whenever a state change occurs. 
using the pseudo-classes:

1.	:hover,
2.	:focus, 
3.	:active,
4.	:target 

Transition properties:
1.	 ## transition-property,
Determines exactly what properties will be altered in conjunction with the other transitional properties.  Only the properties identified will be affected by any transitions. 

NOTE:
Not all properties may be transitioned, for example the display property cannot be transitioned. 

Examples of popular transitional properties 
	background-color
	background-position
	border-color
	border-width
	border-spacing
	bottom
	clip
	color
	crop
	font-size
And many others 

2.	## transition-duration,
 The value of this property can be set using timing values like seconds (s) and milliseconds (ms). 
multiple durations can be declared using comma separated values. The order of these values when identifying individual properties and durations does matter. If multiple properties are being transitioned with only one duration value declared, that one value will be the duration of all the transitioned properties.

3.	## transition-timing-function
Is used to set the speed in which a transition will move.  
You can use:
-	linear, identifies a transition moving in a constant speed from one state to another. 
-	 ease-in,  identifies a transition that starts slowly and speeds up throughout the transition. 
-	ease-out, identifies a transition that starts quickly and slows down throughout the transition. 
-	ease-in-out, identifies a transition that starts slowly, speeds up in the middle, then slows down again before ending.

4.	## transition-delay.
 You can set a delay with a time value (s) or (ms). This determines how long a transition should be stalled before executing.

Note: shorthand transitions
 Using the transition value alone, you can set every transition value in the order of transition-property, transition-duration, transition-timing-function, and lastly transition-delay. Do not use commas with these values unless you are identifying numerous transitions.

-	 CSS3 Animations 
Allow the appearance and behavior of an element to be altered in multiple key frames.  


## Animation keyframes 

To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated. 

## Animation name 
The declared  keyframes need to be assigned to an element.
 To do so, the animation-name property is used with the animation name, identified from the @keyframes rule, as the property value. The animation-name declaration is applied to the element in which the animation is to be applied to.
-	declare an animation-duration property and value so that the browser knows how long an animation should take to complete.

-	Use animation-timing-function to declare timing 

-	Use animation-delay properties to add a delay 

Code example:


@keyframes slide {
0% {
left: 0;
top: 0;
}
50% {
left: 244px;
top: 100px;
}
100% {
left: 488px;
top: 0;
}
}
.stage {
height: 150px;
position: relative;
}
.ball {
height: 50px;
position: absolute;
width: 50px;
}
.stage:hover .ball {
animation-name: slide;
animation-duration: 2s;
animation-timing-function: ease-in-out;
animation-delay: .5s;
}






