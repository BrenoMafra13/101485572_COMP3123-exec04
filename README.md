# 101485572_COMP3123-exec04

A simple Node.js and Express.js project that demonstrates basic REST API design, 
request handling, and serving static files.

# Project Overview

This project shows how to set up an Express.js application with multiple endpoints that handle different types of requests (query parameters, path parameters, and request body). It also includes static middleware to serve an HTML file. It is also a practical example of how to structure and run an Express server.

# Tech Stack

- Node.js
- Express.js
- Nodemon (development auto-reload)

# Setup

- Clone this repository (https://github.com/BrenoMafra13/101485572_COMP3123-exec04.git)
- npm install
- Start the server in development mode: npm run dev
- Run in production mode: npm start
- Open http://localhost:3000 in your browser or test endpoints using Postman/cURL

# API Endpoints

GET /hello
Returns plain text "Hello Express JS"

GET /user?firstname=John&lastname=Doe
Returns a JSON object with firstname and lastname from query parameters.
Defaults to "Breno" and "Lopes Mafra" if none provided.

POST /user/:firstname/:lastname
Returns a JSON object with firstname and lastname from path parameters.

POST /users
Accepts a JSON array of users in the request body and returns the same array.

Static File
Serves instruction.html from the public folder at /instruction.html.
