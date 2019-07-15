# Android_Assignment3 ReadMe file

#Halifax Bus Transit Application

##This is an easy application which can be used to find the buses in
##Halifax which are nearer to your location. This application also helps you 
##find the bus near to your previous location.


###The application loads the google map on its launch and redirects and zoom 
###the map at your device current location. Before launching the map, as a part
###of user security, the application asks for Permission to use access the user
###location. Once the user gives the permission to access the location, the application proceeds further.

###Once the map is loaded, if the application is launched for the first time, the user would be able to see its current location.
But if the application is launched for the second time or more, user would be able to see its previous location.

By clicking the location button avaialble on the top corner, user can see the bus which are available nearby
This bus data is real-time data and it is directly taken from Halifax transit website.

At a time, only bus is visible on the screen since it is real time data and in one 
go data about one bus is fetched and updated. Along with this, the bus location is also updated every 5 secs.

Once the user closes or terminates the application, the application stores the user current location and 
when user opens it for the second time, he would be able to see the previous location and can check for buses by clicking the Location button.

There is only one screen in the application, where in user can perform all the activities. There are two types of marker to showcase the objects.
First one is Location marker which is red in color, the other marker is used to display the bus location.

The application is not crashing anytime and is able to restore the previous location. 

##Wondering how does the application working at backend?

###The application is using Google map and latitude and longitude of the device is being used to identify the current location.
###The real-time data of Halifax bus is fetched from Halifax transit website. http://gtfs.halifax.ca/realtime/Vehicle/VehiclePositions.pb
##Since this is a real-time data it keeps on changing with every second and hence the location of every bus is getting updated with time.
###In the first launch of the application,it takes little time to showcase the bus of the screen and since it's real time application, sometimes it takes 
###to render all the buses of the screen.

On clicking each bus the route number of the bus can be seen. For eg: 1,10,14,9A,9B etc.
The previous marker position of each bus is removed, in order to reduce the complexity over the screen. However that functionality
can be utilized while while tracing the bus path down the project.

#Testing 

In order to test the application, run the application in android phone and then grant permission to access location.
Once that is done, if the application is installed for the first time, you will be able to see current location. 
Press the Location button available on the top, and you will be able to see buses on the screen. 
Sometime, it may take time since it is real time data.

If you press a back button and closes the application, next time when you launch the application, you will be able to see you're
restored location and by clicking the Location button you'll be able to see buses. 
On clicking the bus marker, you can see the bus Route and hence different buses can be identified.

##Note : It is advisable to run the application in Android phone not on emulator. It works best with Android phone and doesnt crashes.

References – 
In order to build the application, following references has been used-
1.	https://stackoverflow.com/questions/17357226/add-the-loading-screen-in-starting-of-the-android-application
2.	https://developers.google.com/maps/documentation/android-sdk/marker
3.	https://developers.google.com/maps/documentation/android-sdk/current-place-tutorial
4.	https://demonuts.com/android-current-location-on-google-map/
5.	https://www.javatpoint.com/android-google-map-displaying-current-location
6.	https://stackoverflow.com/questions/17379807/remove-previous-marker-and-add-new-marker-in-google-map-v2


