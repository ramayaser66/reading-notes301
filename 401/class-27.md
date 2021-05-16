
#  Android Tasks and Back Stack

first: 

` taska:`  a stack of activities that users interact with when performing a certain job. 
The activities are arranged in a stack, in the order in which each activity is opened. 



Note: 
if you opened a new activity and then backed on it this new activity would be popped of the stack and so on. 

 Activities in the stack are never rearranged, only pushed and popped from the stack


- the current activity starts another, the new activity is pushed on the top of the stack 

- The previous activity remains in the stack and the system retains the current state of its user interface, but is stopped 

- using the Back button,  the current activity is popped from the top of the stack AkA destroyed and the previous activity is resumed  AKA restored. 


- using the home button, the current activity is stopped and its task goes into the background. The system retains the state of every activity in the task. If the user later resumes the task by selecting the launcher icon that began the task, the task comes to the foreground and resumes the activity at the top of the stack.

____________________________________________ 


![](https://www.sitepoint.com/wp-content/uploads/2011/07/diagram_backstack1.png)



note that the activities in the back stack are never rearranged this allows to start a particular activity from more than one activity, a new instance of that activity is created and pushed onto the stack rather than bringing any previous instance of the activity to the top.

one activity in your app might be instantiated multiple times, you can modify it if you do not want an activity to be instantiated more than once.

## Managing Tasks 

default: the back stack all activities started in succession in the same task and in a "last in, first out. 

you can control the behavior by using the principle activity attributes like, 

- taskAffinity
- launchMode
- allowTaskReparenting
- clearTaskOnLaunch
- alwaysRetainTaskState
- finishOnTaskLaunch
- FLAG_ACTIVITY_NEW_TASK
- FLAG_ACTIVITY_CLEAR_TOP
- FLAG_ACTIVITY_SINGLE_TOP


## Android SharedPreferences

A SharedPreferences object points to a file containing key-value pairs and provides simple methods to read and write them.
 Each SharedPreferences file is managed by the framework and can be private or shared.

 creating a shared preference file:

 - getSharedPreferences() 
 multiple shared preference files 

 - getPreferences()  
  one shared preference file 