#  The past, present and future off local storage for web applications 

_______________________________________________________________________________________________


> ## persistent local storage

-	native client applications 
the operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state. These values may be stored in the registry, INI files, XML files, or some other place according to platform convention. If your native client application needs local storage beyond key/value pairs, you can embed your own database, invent your own file format, or any number of other solutions. 

-	web applications 
 web applications had none of these luxuries. Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data. But they have three potentially downsides:


1.	Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over

2.	Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)


3.	Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful

What we want :
-	A lot of storage space
-	 the client
-	 persists beyond a page refresh
-	And isn’t transmitted to the server

None of these were accomplished before html 5

## A brief history of local storage hacks before html5


-	Internet Explorer. 
Microsoft invented many things and included them in their browser Internet Explorer. One of these things was called DHTML Behaviors, and one of these behaviors was called userData which allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure. (Trusted domains, such as intranet sites, can store 10 times that amount. IE does not present any form of permissions dialog, and there is no allowance for increasing the amount of storage available.


-	Flash 

![flash](https://www.welivesecurity.com/wp-content/uploads/2014/11/Adobe-flash-exploit-kit.jpg)



Adobe introduced Local Shared Objects which allows Flash objects to store up to 100 KB of data per domain. An early prototype of a Flash-to-JavaScript bridge called AMASS (AJAX Massive Storage System) was developed but it was limited by some of Flash’s design quirks. 
Then in flash 8 with the advent of ExternalInterface accessing LSOs from JavaScript became an order of magnitude easier and faster. AMASS was rewritten and integrated it into the popular Dojo Toolkit under the moniker dojox.storage 
So flash give each domain 100 KB of storage “for free.”  And 
It prompted the user for each order of magnitude increase in data storage (1 Mb, 10 Mb, and so on). 
The work on dojox.storage continued to provide a unified interface to all these different plugins and APIs.  Until it was able to auto-detect (and provide a unified interface on top of) Adobe Flash, Gears, Adobe AIR, and an early prototype of HTML5 storage that was only implemented in older versions of Firefox.

-	Gears 
![gears](https://image.slidesharecdn.com/going-offline-with-gears-and-gwt-1201451770307347-2/95/going-offline-with-gears-and-gwt-12-728.jpg?cb=1201422971)


Google launched Gears, which is an open source browser plugin provides additional capabilities in browsers.  Gears provides an API to an embedded SQL database based on SQLite. After obtaining permission from the user once, Gears can store unlimited amounts of data per domain in SQL database tables.



> # HTML5 Storage 

![html5](https://www.diygenius.com/wp-content/uploads/2013/07/learn-html5.jpg)  

<br> 

HTML5 Storage” is a specification named Web Storage , 
which was part of the HTML5 specification proper, but was split out into its own specification . browser vendors refer to it as “Local Storage” or “DOM Storage.”

Html5  is  a way for web pages to store named key/value pairs locally, within the client web browser. this data persists even after you navigate away from the web site, close your browser tab or exit your browser. 
This data is never transmitted to the remote web server or you can send it manually.  Unlike all previous attempts at providing persistent local storage, it is implemented natively in web browsers, so it is available even when third-party browser plugins are not.

## using html5 storage 
HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. 
-	The named key is a string.
-	The data can be any type supported by JavaScript, including:
1.	strings,
2.	Booleans, 
3.	Floats
the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype. 
-	setItem() 
Calling setItem() with a named key that already exists will silently overwrite the previous value. 
-	 getItem() 
Calling getItem() with a non-existent key will return null rather than throw an exception. 
-	removeItem() 
 removing the value for a given named key, and clearing the entire storage area. 
Calling removeItem() with a non-existent key will do nothing. 

-	key() 
Get the total number of values in the storage area, and to iterate through all of the keys by index. 
If you call key() with an index that is not between 0–(length-1), the function will return null. 

## tracking changes to the html5 storage area 
-	storage event 
The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something. 
to hook the storage event, you’ll need to check which event mechanism the browser supports.  
Note: 
if you set an item to its existing value or call clear() when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area. 


## limitations in current browsers 
-	limitations of the now-standardized HTML5 Storage. 

1.	5 megabytes 
How much storage space each origin gets by default. 
 One thing to keep in mind is that you’re storing strings, not data in its original format. If you’re storing a lot of integers or floats, the difference in representation can really add up. Each digit in that float is being stored as a character, not in the usual representation of a floating point number
2.	QUOTA_EXCEEDED_ERR 
the exception that will get thrown if you exceed your storage quota of 5 megabytes. And you can’t ask the user for more storage space 

## HTML5 Storage space 
 if you close the browser window after a few changes and you didn’t complete, you’ll lose your progress. But with HTML5 Storage, we can save the progress locally, within the browser itself. Make a few changes, then close the browser tab, then re-open it. If your browser supports HTML5 Storage, the demonstration page should magically remember your latest moves.  Using the proper function 









