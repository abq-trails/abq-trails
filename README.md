### Team Roster 
[Alana Chigbrow](https://github.com/achigbrow)   
[Anita Martin](https://github.com/anita-martin5703) 
[Denelle Linebarger](https://github.com/DBrittonLinebarger)   
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

## External data & services

We plan to use the following data sources and services:

* Albuquerque Open Space and Open Trails datasets.
* Google Maps API.
* Google Sign-In for authentication (unauthenticated users will still be able to browse, but not post comments, ratings, or photos).

### More Information

* [User Stories](docs/user-stories.md)
* [Wireframes](docs/wireframes.md)
* [Ground Rules](docs/ground-rules.md)
* [Front End ERD](docs/erd-front-end.md)
* [Back End ERD](docs/erd-back-end.md)
