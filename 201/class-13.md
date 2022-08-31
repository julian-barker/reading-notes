[Home](../README.md)

# Class 13

## Local Storage

- Local Storage is a way of preserving state for a user without necessarily needing to use a server and login
- Cookies are the standard way of achieving this. They are useful tooltext files on the users computer that connect to the site domain. some limitations are:
  - They burden every page on the domain
  - They only store up to 4KB
  - They are often turned off or blocked because they are associated with privacy and security concerns

- To help solve this, some local storage specs were added to HTML.
- access the localStorage object in JS with the `localStorage.getItem(key)` and `localStorage.setItem(key, value)` methods.
- Remove items with the `.removeItem(key)` method.
- `sessionStorage functions similarly, but only stores information for as long as the page is open, meaning it will still preserve data through refreshes.
- Local storage can only store strings, so to be able to store more complex data types, we use the `JSON.stringify()` and `JSON.parse()` methods

### Use Cases

1. One nice use case is caching web service data to LocalStorage to reduce successive page load times
  - ajax() > getJSON for web services

2. We can use local Storage to maintain state, either by maintaining the status of the HTML, or by storing an object with the setting values for all of the dynamic site components
