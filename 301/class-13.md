[Home](../README.md)

# Class 13

## CRUD

1. Which HTTP method would you use to update a record through an API?
  You would use the PUT or PATCH method depending on if it is a partial or full update.

2. Which REST methods require an ID parameter?
  PUT, PATCH, DELETE. GET can take an id but defaults to getting all data if omitted.

## Building a CRUD API

1. What’s the relationship between REST and CRUD?
  POST -> Create
  GET -> Read
  PUT / PATCH -> Update
  DELETE -> Delete

2. If you had to describe the process of creating a RESTful API in 5 steps, what would they be?

      i. Create server
        
      ii. Configure middleware

      iii. Set up Routes
      
      iv. Set up functions based on routes

      v. Set up error handling
