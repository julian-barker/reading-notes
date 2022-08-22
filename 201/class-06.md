[Home](../README.md)

## Class 06

### Objects

- A javascript object is a collection of related data and/or functions. For example, you could build an object to represent a person, and have properties under that object that represent the name, age, height, and favorite color.
- Objects are created with a variable name (generally with a capitalized first letter) and curly braces
- An object literal allows us to convey information more efficiently than sending individual variables, and it allows us easier access to data than an array does, in that its information is labeled. Thus you don't have to search through the contents of the array to find what you are looking for.
- In arrays, we can only access information by its index in the array
- An object literal is contrasted with an object that is instantiated from a class, or generic representation of that object.
- Dot notation allows us to access object methods and properties by calling the name of the object, a period, and the name of the property (i.e. Person.age). functions, as normal, use parentheses at the end, even in the absence of arguments.
- Objects can be nested, and have other objects as properties.
- Dot notation is useful, but not always possible. When using objects within functions, if you need to pass a variable to an object to determine what property to access, you need to use bracket notation (i.e Person[input])
- the keyword `this` refers to the parent object when used inside a function property.

### The DOM

- DOM stands for Document Object Model
- The DOM represents the page so that its structure and appearance can be changed
- Critically, it allows javascript to interact with and modify the page
- The `document` object represents the page in its entirety
- The DOM is not javascript, but is a web API that javascript uses to interact with the page.