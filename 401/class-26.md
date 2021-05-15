

# Android Fundamentals 

![](http://1.bp.blogspot.com/-ox9b54FkhHo/UdqduQ0dEaI/AAAAAAAABj4/nGZnO31wu7g/s1600/Android+Application+Fundamentals+and+Components.jpg)


you can write an Android app using: 
-  Kotlin language
-  Java language
-  C++ language 


 Android security features:

 -  Android operating system, 
a multi-user Linux system in which each app is a different user.

-  a unique Linux user ID, 
The system sets permissions for all the files in an app so that only the user ID assigned to that app can access them.

-  virtual machine, 
Each process has its own virtual machine (VM), so an app's code runs in isolation from other apps. 

- every app runs in its own Linux process

 each app, by default, has access only to the components that it requires to do its work, an app cannot access parts of the system for which it is not given permission.

 You can share data between apps by: 
- let the two apps to share the same Linux user ID

- An app can request permission to access device data 

## app components 

- Activities
the entry point for interacting with the user. 


- Services
 a component that runs in the background to perform long-running operations or to perform work for remote processes.
 Note:  A service does not provide a user interface
- Broadcast receivers
a component that enables the system to deliver events to the app outside of a regular user flow, allowing the app to respond to system-wide broadcast announcements.
 the system can deliver broadcasts even to apps that aren't currently running. 
- Content providers
a shared set of app data that you can store in the file system. 
 other apps can query or modify the data if the content provider allows it.


 ## Activating components 
]activities, services, and broadcast receivers—are activated by an asynchronous message called an `intent`

Intents bind individual components to each other at runtime. 
They are the messengers that request an action from other components, whether the component belongs to your app or another.

## The manifest file 

reading the app's manifest file allows the Android system to start the app component. that way it knows that the component exists. 
the manifest: 
1.  declares all its components in this file 
2. Identifies any user permissions the app requires, such as Internet access or read-access to the user's contacts.
3. Declares the minimum API Level required by the app, based on which APIs the app uses. 
4. Declares hardware and software features used or required by the app, such as a camera, bluetooth services, or a multitouch screen.
5. Declares API libraries the app needs to be linked against (other than the Android framework APIs)


