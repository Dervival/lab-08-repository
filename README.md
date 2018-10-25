# lab-08-repo
Repository for Seattle-301d39's series of labs focusing on server and API usage
**Author**: Patrick McNamee and Blaise Clarke (Thursday)
            Blaise Clarke and Carlos Castillo (Wednesday)
**Version**: 1.1.0 

## Overview
This application accepts a location from a user and provides relevant information to the location (a list of restaurants, movies set there, and the current week's weather) using APIs. If the location has been searched previously, a cached version of the location is used instead. This application helps tourists and local people plan their time in the city more effectively.

## Getting Started
+ First, go to the application's front end at https://codefellows.github.io/city_explorer/
+ Ensure your versions of node, NPM, and nodemon are up to date
+ Next, fork or clone this repository in a folder locally
+ In that folder, initialize NPM with npm init. Modify the package.json created by this to include the below dependencies
+ Then, install dependencies express, superagent, dotenv, and cors in the same repository. 
+ Set your environmental variable for PORT to 3000.
+ To test the application, type 'nodemon' in the console while in the same directory as server.js
+ Then enter http://localhost:3000 into the field showing on the front end.
+ Type in a city, and infomation will populate below.

## Architecture
This application is written in Javascript. We are using AJAX calls to read in from APIs and send it to the front-end for showing templates.

## Change Log
10-25-2018 01:25pm - Generic functionality incomplete, but no time left for bugfixing or refactoring; reverting to previous stable version and submitting.
10-25-2018 11:33am - Initial concept of generic functionality for weather, yelp, and movies API completed.
10-25-2018 10:54am - Initial deployment to Heroku
10-25-2018 10:42am - Added utility to use cached data from location table in the database.
10-25-2018 10:30am - Added postgres database and ability to save data to it.
10-24-2018 01:40pm - Application now can display movie information that uses the city name as a filter. Turning in now.
10-24-2018 01:03PM - Proof of life of TMDB (The Movie database) API.
10-24-2018 11:30AM - Added functionality with the Yelp API to return restaurant information.
10-24-2018 10:34AM - Refactored weather data to return normalized data through the use of .map functionality.
10-24-2018 10:26AM - Weather data has been replaced with the use of the Dark Sky API.
10-24-2018 10:05AM - Location data has been replaced with usage of a Google API. Application has been published to Heroku in a partial state.
10-24-2018 - Application can read from json files.

## Credits and Collaborations
Thanks to Patrick McNamee for the refactoring of location access as well as the idea to genericize other API calls/database queries.
Thanks to Carlos Castillo for the creation of server.js as well as coordinating API keys for this project.
