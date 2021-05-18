# jobly-backend

## Introduction 
This is a Node.js/Express.js backend for my full-stack job search web application, Jobly. It includes a classic RESTful API setup for storing and providing information on companies, jobs, and users. 

Backend can be accessed using the following link: https://alexgenc-jobly.herokuapp.com/ 

## Routes

- /auth - Used for user authentication and authorization, i.e., user sign up and sign in.
- /companies - A list of companies in the database
- /jobs - A list of jobs in the database
- /users - A list of users in the database. Only available for admin users.

## Database

Backend is connected to a PostgreSQL database. All company and job related information, as well as user information (after encrypting with Bcrypt) are stored in the database.

## Error Handling and API Query Validation

The backend is configured to throw specific errors for 404(NOT_FOUND), 401(UNAUTHORIZED), 400(BAD REQUEST), 403(FORBIDDEN), and a general error handler for all remaining cases.

API Query validation is accomplished using JSON Schema. There is a specific schema file for every model activity in the /schemas folder that must be matched when making requests to the API.

## Testing

All models, routes, middleware, and helper files are tested for full coverage.




