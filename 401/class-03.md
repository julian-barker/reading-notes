[Home](../README.md)

# Class 3

## ES6 Classes

- Classes in Javascript are a template for creating objects.
- They are just special functions
- Unlike functions, however, class hoisting does not work in the same way as normal function hoisting. That is, they cannot be used or called before above the class declaration. While the class variable wil be declared and hoisted, it will not be initialized until its spot in the code.
- A constructor in a class is just a function that gets called every time a new instance of the class is created. It serves to initialize properties in the class, with or without some inputs to the constructor.
- Contextual `this` refers to the `this` object within a class pointing to the instance of that class. `this` in JS means different things in different contexts, but by default, it refers to either the top level execution context or the object on which the function is called, if the function is a method.

## Using Express Routing

- Within Express, routing refers to how an application's endpoints handle and respond to different requests
- A route method refers to an implementation of one of the HTTP methods, such as GET or POST, whereas a route path builds on that to include the URI in conjunction with the method.
- It is appropriate to add next as a parameter to your route handler if it will be followed by another function. This function could be a piece of middleware or an error handler.

## Express Routing

- An express router is similar to an express app, but slightly pared down.  I tprovides the main functionality of the express application API, such as `.get`, `.use`, `.param`, and `.route`
- We can implement route-level middleware with `router.use()` to specify middleware to run specifically routes using this router, but on all its methods/routes.
