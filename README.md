### Team Roster 
[Alana Chigbrow](https://github.com/achigbrow)   
[Anita Martin](https://github.com/anita-martin5703)   
[Denelle Britton Linebarger](https://github.com/DBrittonLinebarger)   
[David Nelson](https://github.com/djpn/)

## Summary

A combination of a server platform and a mobile app, allowing users to browse/search the open space trails in the Albuquerque area, ask questions of other users, leave comments, post pictures, rate of any given trail, and review the aggregate ratings from the community.

## Why

There is a wealth of beautiful open space in and around Albuquerque. In addition, data on open spaces and trails is part of the Albuquerque Open Data project. However, there's not a convenient web site or application for browsing this information; nor is there any particular facility for members of the community to provide input, share experiences, share photos, etc.

## Who

This app would be targeted to locals and visitors who want to explore the Albuquerque open space, and who would like to be informed/prepared prior to setting out. It is also aimed at members of the community who want to share their explorations and experiences with others.

## What runs where?
### Cloud

The cloud side of this system (currently expected to be implemented using the Spring Boot Java enterprise platform) would provide the searchable repository of user comments, ratings, and photographs. This data would reference data obtained from the Albuquerque Open Space and Open Trails datasets.

### User App

The user app (currently planned for implementation on the Android platform) would provide a browsing/searching interface to the dataset of open space trails, as well as a Google Maps-based view of their locations. If there's a live connection to the cloud side of the system, comments, ratings, and photos would also be available. (Currently, we plan to access the Albuquerque Open Space and Open Trails datasets directly from the user app, so that there would be some functionality available, even if the server side of the system is down.)


## Functional Inventory  

### Back End    

- Apache HTTP server  ??
- Apache Tomcat Java Application server/container  ??
- Web service application, incorporating:  
\* Data model    
  * Embedded Apache Derby database ??
  * Hibernate ORM  
  * Custom entity classes 
  * Spring Boot Data  
  * Custom data repository interfaces  
\* Service Controllers  
  * Spring MVC  
  * Custom controller classes  
\* View Composition & serialization  
  * Jacskon JSON  
  * Custom view classes and interfaces  
\* Authentication  
  * Spring Security  
  * Google Sign In


OMG CORBA API ??

#### Third Party Libraries
* Room Persistence Library  
* Stetho    
* Spring Framework
* Gson ??  
* MySQL    
* Jackson  
* GeoJson  


### Front End   

\* Data model 
  * Custom entity classes 

\* Service controllers   
  * Custom controller classes  

\* View composition and serialization 
  * Custom view classes and interfaces

\* Authentication  
  * Google Sign In




#### Third Party Libraries
* Room Persistence Library  
* Stetho  
* Gson  
* Reactivex  
* Retrofit2
* RxJava ??  
* Espresso ??  
* SQL Lite ??



## Current State of Completion  


## Aesthetic/Cosmetic Improvements for Front End  

## Functional Stretch Goals  


## Platforms Used/Restrictions


### API Versions and Hardware   
* Compiled Sdk version 28 ??  
* Minimum Sdk version 21  
* Targeted Sdk version 29  
* Version code 1  
* VersionName "1.0"  
* Emulator: Nexus 5X API 28 ?? others??  



## External data & services

* Albuquerque Open Space and Open Trails datasets.
* Google Maps API.
* Google Sign-In for authentication (unauthenticated users will still be able to browse, but not post comments, ratings, or photos).    



### Links

* [User Stories](docs/user-stories.md)
* [Wireframes](docs/wireframes.md)
* [Ground Rules](docs/ground-rules.md)
* [Front End ERD](docs/erd-front-end.md)
* [Back End ERD](docs/erd-back-end.md)  
* DDL
* Licenses/Copyrights  
* Javadoc  
* Documentation for Web Services  
* Build and Deployment Instructions for Back End/Front End  
* Basic User Instructions  


