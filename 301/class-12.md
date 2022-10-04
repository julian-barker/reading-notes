[Home](../README.md)

# Class 12

## REST Status Codes

1. In your own words, describe what each group of status code represents:

- 100’s = informational status codes
- 200’s = success codes
- 300’s = redirect codes
- 400’s = client-side errors
- 500’s = server-side errors

2. What is a status code 202?
  `202` means accepted, which says that a request has been recieved, but the response will come some time later.

3. What is a status code 308?
  `308` is a permanent redirect and tells the client to look for the requested data at a new location.

4. What code would you use if an update didn’t return data to a client?
  `204` - no content

5. What code would you use if a resource used to exist but no longer does?
  `410` gone

6. What is the ‘Forbidden’ status code?
  `403` - the client has no permissions to access the content

## MERN Video

1. Why do we need to pull our MongoDB database string out of our server and put it into our `.env`?
  We don't want to expose that to the public and to the client. `.env` does not get pushed to github. furthermore, ,it allows that variable to be changed if necessary, without changing the code.

2. What is middleware?
  Middleware is code that runs after receiving a request but before passing it to the server routes.

3. What does `app.use(express.json())` do?
  It sets up the server to use JSON as return data from a request.

4. What does the `/:id` mean in a route?
  `/:id` refers to a parameter passed in to get a specific piece of data. It can be accessed with `req.query.params`.


5. What is the difference between `PUT` and `PATCH`?
  `PUT` updates a piece of data to a new value, while `PATCH` is only a partial update to a piece of data.

6. How do you make a default value in a schema?
  You add a `default` field in the properties object for a key

7. What does a `500` error status code mean?
  `Internal Server Error`, this can actually result from a client-side error if the request was never validated.

8. What is the difference between a status `200` and a status `201`?
  `201` is specifically returned after something is successfully created.
