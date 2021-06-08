# Intent Filter

an expression in an app's manifest file that specifies the type of intents that the component would like to receive

`Intent Filter -->` a respond to action requests.
perform an action that might be useful from another app,

![](https://i.ytimg.com/vi/qohEYaOqiXY/maxresdefault.jpg)



An `Intent` is an object passed to Context. startActivity(),Context. ... 
While `Intent filter` are used for broadcast receiver. Whenever the intent filter condition is match the android OS will launch that activity.


- An intent filter declares the capabilities of its parent component — what an activity or service can do and what types of broadcasts a receiver can handle. It opens the component to receiving intents of the advertised type, while filtering out those that are not meaningful for the component

- you will need an <intent-filter> element in your manifest file for the corresponding <activity> element. 

-  each intent filter you add should be as specific as possible in terms of the type of action and data the activity accepts. 

if that activity has an intent filter it must have the criteria of the Intent object:

- Action
- Data
- Category


## Handle the Intent in Your Activity 
As your activity starts, call getIntent() to retrieve the Intent that started the activity on onCreate() or onStart().



## Return a Result

`setResult()` to specify the result code and result Intent.
then call `finish()` to close (and destroy) your activity.


Note: You must always specify a result code with the result. Generally, it's either RESULT_OK or RESULT_CANCELED 

