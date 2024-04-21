# LightBnB

Welcome! LightBnB is a vacation rental platform that allows homeowners to rent out their properties to travelers. It provides an alternative to traditional hotels and bed and breakfasts, offering a unique and personalized experience for both hosts and guests.

## Features
**Search**: Travelers can easily search for properties based on their preferences. <br>
**List Your Property**: Homeowners can list their properties, providing detailed information such as location, amenities, and pricing. <br>
**Listing Management**: Users can view and manage their reservations. <br>
**Reservation Management**: Users can view and manage their reservations.

## Preview
Once you log in, you can view all the listings

!["Landing Page"](https://github.com/cynthia-lam/LightBnB/blob/master/LightBnB_WebApp/docs/LightBnB%20homepage%20logged%20in.png)

Use the "Create Listing" link and fill out this form to post your property

!["Create Listings"](https://github.com/cynthia-lam/LightBnB/blob/master/LightBnB_WebApp/docs/LightBnB%20create%20listing.png)

Here, users can filter listings by their preferences

!["Search Page"](https://github.com/cynthia-lam/LightBnB/blob/master/LightBnB_WebApp/docs/LightBnB%20search.png)

An example of search results
!["Search Reults"](https://github.com/cynthia-lam/LightBnB/blob/master/LightBnB_WebApp/docs/LightBnB%20search%20results.png)

Users can also manage their listings and reservations

!["My Listings"](https://github.com/cynthia-lam/LightBnB/blob/master/LightBnB_WebApp/docs/LightBnB%20my%20listings.png)

## Installation
To run LightBnB locally, follow these steps:

1. Install dependencies: ```npm install```
2. Start the server: ```npm run local```
3. Access the application in your browser at http://localhost:3000

## Project Structure
* `db` contains all the database interaction code.
  * `json` is a directory that contains a bunch of dummy data in `.json` files.
  * `database.js` is responsible for all queries to the database. It doesn't currently connect to any database, all it does is return data from `.json` files.
* `public` contains all of the HTML, CSS, and client side JavaScript. 
  * `index.html` is the entry point to the application. It's the only html page because this is a single page application.
  * `javascript` contains all of the client side javascript files.
    * `index.js` starts up the application by rendering the listings.
    * `network.js` manages all ajax requests to the server.
    * `views_manager.js` manages which components appear on screen.
    * `components` contains all of the individual html components. They are all created using jQuery.
* `routes` contains the router files which are responsible for any HTTP requests to `/users/something` or `/api/something`. 
* `styles` contains all of the sass files. 
* `server.js` is the entry point to the application. This connects the routes to the database.
