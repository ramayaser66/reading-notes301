
# location

you can request the last known location of the user's device `-->` using the Google Play services location APIs.


- **` fused location provider`** 

 one of the location APIs in Google Play services, it retrieves the device's last known location.

  using the `getLastLocation()` method in the fused location provider.


  ## Set up Google Play services

   Download and install the Google Play services component via the SDK Manager and add the library to your project. 

   ## Specify app permissions
   `-->` request location permissions.

  ## Create location services client

  ## Get the last known location

  -  use  `getLastLocation()`, to retrieve the device location


   Note: The precision of the location returned by this call is determined by the permission setting you put in your app manifest. 

   this method returns a Task that you can use to get a Location object with the latitude and longitude coordinates of a geographic location.


**The location object may be null in the following situations:**

- `Location is turned off in the device settings` The result could be null even if the last location was previously retrieved because disabling location also clears the cache.

- The device never recorded its location, which could be the case of a `new device` or a device that has been `restored to factory settings.`

- Google Play services on the device has restarted, and there is no active Fused Location Provider client that has requested location after the services restarted.



## Maintain a current best estimate 

the accuracy of a location varies, the most recent value isn't necessarily the best. You should include logic for choosing which location to show based on several criteria. 


to validate the accuracy of a location:
- Check whether the location retrieved is significantly newer than the previously fetched location.

- Check whether the accuracy claimed by the location is better or worse than that of the previous estimate.

- Check the provider that's associated with the new location. Decide whether you trust this provider more than the one used in your app's cached location.