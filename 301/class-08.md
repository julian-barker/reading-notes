[Home](../README.md)

# Class 08

## REST APIs

1. What does REST stand for?
  "Representational State Transfer"

2. REST APIs are designed around a ____.
  Resource - any kind of object, data, or service that can be accessed by the client

3. What is an identifier of a resource? Give an example.
  A URI that uniquely identifies that resource, which looks similar to a standard URL. The provided example is for a customer order: `https://adventure-works.com/orders/1`

4. What are the most common HTTP verbs?
  `GET`, `POST`, `PUT`, `PATCH`, `DELETE`

5. What should the URIs be based on?
  URIs should have a consistent naming convention based on nouns.

6. Give an example of a good URI.
  `https://adventure-works.com/orders` - Avoid creating APIs that simply mirror the internal structure of a database.

7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
  Chatty APIs expose a large number of resources - they are not concise in their responses. This places a larger load on servers and is generally a bad thing.

8. What status code does a successful `GET` request return?
  200 (OK)

9. What status code does an unsuccessful `GET` request return?
  404 (Not Found)

10. What status code does a successful `POST` request return?
  Good - 201 (Created) / Bad - 400 (Bad Request)

11. What status code does a successful `DELETE` request return?
  Good - 204 (No Content) / Bad - 404

***

### More

- `GET` retrieves a representation of the resource at the specified URI. The body of the response message contains the details of the requested resource.
- `POST` creates a new resource at the specified URI. The body of the request message provides the details of the new resource. Note that POST can also be used to trigger operations that don't actually create resources.
- `PUT` either creates or replaces the resource at the specified URI. The body of the request message specifies the resource to be created or updated.
- `PATCH` performs a partial update of a resource. The request body specifies the set of changes to apply to the resource.
- `DELETE` removes the resource at the specified URI.

- *** PUT requests must be idempotent. If a client submits the same PUT request multiple times, the results should always be the same (the same resource will be modified with the same values). POST and PATCH requests are not guaranteed to be idempotent.
