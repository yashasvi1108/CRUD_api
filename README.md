# CRUD_api

Movie API
This is a RESTful API built with Go (Golang) using the Gorilla Mux package. It provides endpoints to perform CRUD operations (Create, Read, Update, Delete) on a collection of movie resources. The API allows users to interact with the data in a structured and consistent way.

Endpoints
GET /movies - Retrieves all movies in the collection
GET /movies/{id} - Retrieves a specific movie by its ID
POST /movies - Creates a new movie resource
PUT /movies/{id} - Updates an existing movie resource
DELETE /movies/{id} - Deletes a specific movie by its ID
Movie Resource
A movie resource is represented by a JSON object with the following fields:

id - A unique identifier for the movie
isbn - The International Standard Book Number (ISBN) for the movie
title - The title of the movie
director - An object containing information about the director of the movie, with the following fields:
firstname - The first name of the director
lastname - The last name of the director

Usage
To use this API, start the server by running the following command:
go run main.go

This will start the server on port 8000.

Once the server is running, you can interact with the API using a tool like curl or a web-based API client like Postman.

For example, to retrieve all movies in the collection, send a GET request to http://localhost:8000/movies. To create a new movie resource, send a POST request to http://localhost:8000/movies with a JSON payload representing the new movie.

Dependencies
This API relies on the following dependencies:

Gorilla Mux - A powerful HTTP router and URL matcher for building Go web servers.
These dependencies can be installed using the following command:
go get github.com/gorilla/mux

