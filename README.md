### Team Roster 
[Alana Chigbrow](https://github.com/achigbrow)   
[Anita Martin](https://github.com/anita-martin5703)   
[Denelle Britton Linebarger](https://github.com/DBrittonLinebarger)   
[David Nelson](https://github.com/djpn/)  

## Primary Responsibilities  
 Alana Chigbrow: Backend Database  
 Anita Martin: Google Maps with Trails    
 Denelle Britton Linebarger: Documentation/Trail Reviews    
 David Nelson: Trail View   
 

## Summary

A combination of a server platform and a mobile app, allowing users to browse/search the open space trails in the Albuquerque area, ask questions of other users, leave comments, post pictures, rate of any given trail, and review the aggregate ratings from the community.

## Why

There is a wealth of beautiful open space in and around Albuquerque. In addition, data on open spaces and trails is part of the Albuquerque Open Data project. However, there's not a convenient web site or application for browsing this information; nor is there any particular facility for members of the community to provide input, share experiences, share photos, etc.

## Who

This app is targeted to locals and visitors who want to explore the Albuquerque open space, and who would like to be informed/prepared prior to setting out. It is also aimed at members of the community who want to share their explorations and experiences with others.

## What runs where?
### Cloud

The cloud side of this system (currently expected to be implemented using the Spring Boot Java enterprise platform) provides the searchable repository of user comments, ratings, and photographs. This data references data obtained from the Albuquerque Open Space and Open Trails datasets.

### User App

The user app (implementated on the Android platform) provides a browsing/searching interface to the dataset of open space trails, as well as a Google Maps-based view of their locations. If there's a live connection to the cloud side of the system, comments, ratings, and photos would also be available. (Currently, we plan to access the Albuquerque Open Space and Open Trails datasets directly from the user app, so that there would be some functionality available, even if the server side of the system is down.)


## Functional Inventory  

### Back End    

- Web service application, incorporating:   
    * Data model    
      * Hibernate ORM    
      * Custom entity classes   
      * Spring Boot Data    
      * Custom data repository interfaces    
   * Service Controllers  
       * Spring MVC  
       * Custom controller classes  
   * View Composition & serialization  
      * Jacskon JSON  
       * Custom view classes and interfaces  
   * Authentication  
        * Spring Security  
        * Google Sign In


- Third Party Libraries  
        * Room Persistence Library        
        * Stetho      
        * Spring Framework      
        * MySQL      
        * Jackson  
        * GeoJson  


### Front End   

* Web service application incorporating
    * Data model 
      * Custom entity classes 

   * Service controllers   
      * Custom controller classes  

   * View composition and serialization 
      * Custom view classes and interfaces

   * Authentication  
      * Google Sign In



* Third Party Libraries
      * Room Persistence Library  
      * Stetho  
      * Gson  
      * Reactivex  
      * Retrofit2  
      * RxJava  
      

## Current State of Completion
The backend server's MySQL database is running on an external server located at abqtrails.chigbrowsoftware.com. We still need to deploy the entire backend to that server as the Spring application still needs to be run locally. Furthermore, we have to complete the tests which exist only as a framework as of this date.

The app connects to the server and populates its room database from the back end server. It provides a map view with the trails displayed. You can click on a trail to open its individual view. That view is currently under construction.

Please see the below sections for planned completion improvements.


## Aesthetic/Cosmetic Improvements for Front End
- Hide the MapActivity while viewing a TrailViewFragment and the Subsequent UserRatingFragment
- Make different trails noticeably different colors
- Serachbar and button to work where it updates the markers shown based on user input
- Add in a launcher Icon

## Functional Stretch Goals
 - Get the backend and the front end to communicate properly and accept front end sent user reviews.
 - Disallow the user from sending more than one review per click of "Add a rating" found in the TrailViewFragment.
 - Allow a user to go back from a specific trail view to the map so they can view a different trail's view.


## Platforms Used/Restrictions


### API Versions and Hardware   
* Compiled Sdk version 29  
* Minimum Sdk version 21  
* Targeted Sdk version 29  
* Version code 1  
* VersionName "1.0"  
* Emulator: Nexus 5X API 28  



## External data & services

* Albuquerque Open Space and Open Trails datasets.
* Google Maps API.
* Google Sign-In for authentication (unauthenticated users will still be able to browse, but not post comments, ratings, or photos).    



### Links

* [User Stories](docs/user-stories.md)
* [Wireframes](docs/wireframes.md)
* [Ground Rules](docs/ground-rules.md)
* [Front End ERD](docs/finalfe.png)
* [Back End ERD](docs/BackEndERD080719.png)  
* DDL
* [Licenses/Copyrights](docs/licenses-and-copyrights.md)
* [Clientside Javadoc](abq-trails-client-side/docs/api/overview-summary.html)
* Javadoc
* Documentation for Web Services   
* [ABQ opentrails Dataset](http://data.cabq.gov/community/opentrails/trail_segments.geojson)  
* [ABQ opentrails MetaData](http://data.cabq.gov/community/opentrails/MetaData.pdf/)  
* [Google Maps Documentation](https://developers.google.com/maps/documentation/android-sdk/intro)  
* [Android 'Room Database Documentation](https://developer.android.com/topic/libraries/architecture/room)  
* [Build and Deployment Instructions for Back End/Front End](docs/build_user_instructions.md)
* [Basic User Instructions](docs/user_instructions.md)
