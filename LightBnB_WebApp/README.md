# LightBnB

Practice with SQL integration into a javascript database.

## Description

This application is a simplicated spinoff of the popular short term booking app.

## Getting Started

### Dependencies

* bcrypt: ^3.0.6
* cookie-session: ^1.3.3
* express: ^4.17.1
* nodemon: ^1.19.1

### Installing

* Download from github

### Executing program

* Clone this repostory
```
git clone git@github.com:lunamoonmoon/LightBnB.git
cd lightbnb
```
* Install required packages
```
npm install
```
* Connect to the server
```
npm start
```
* Go to localhost:3000 in your browser

## Authors

Contributors names and contact info

[lunamoonmoon](https://github.com/lunamoonmoon)
[lighthouse-labs](https://github.com/lighthouse-labs/LightBnB_WebApp)

## Acknowledgments

Starter code, inspiration, code snippets, etc.
[lighthouse-labs](https://github.com/lighthouse-labs/LightBnB_WebApp)

## Project Structure

```
.
├── db
│   ├── json
│   └── database.js
├── public
│   ├── javascript
│   │   ├── components 
│   │   │   ├── header.js
│   │   │   ├── login_form.js
│   │   │   ├── new_property_form.js
│   │   │   ├── property_listing.js
│   │   │   ├── property_listings.js
│   │   │   ├── search_form.js
│   │   │   └── signup_form.js
│   │   ├── libraries
│   │   ├── index.js
│   │   ├── network.js
│   │   └── views_manager.js
│   ├── styles
│   │   ├── main.css
│   │   └── main.css.map
│   └── index.html
├── routes
│   ├── apiRoutes.js
│   └── userRoutes.js
├── styles  
│   ├── _forms.scss
│   ├── _header.scss
│   ├── _property-listings.scss
│   └── main.scss
├── .gitignore
├── package-lock.json
├── package.json
├── README.md
└── server.js
```

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
