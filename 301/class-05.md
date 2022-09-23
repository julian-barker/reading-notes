[Home](../README.md)

# Class 05

## Thinking in React

1. What is the single responsibility principle and how does it apply to components?
  The dsingle responsibility principle says that a component should ideally only do one thing. If it's scope grows, it should be broken into smaller components.
2. What does it mean to build a ‘static’ version of your application?
  A static build is one in which none of the components have dynamic functionality. It is essentially the HTML representation of you page on load. For this, you will not use state at all.
3. Once you have a static application, what do you need to add?
  We need to add state to be able to trigger changes in the app.
4. What are the three questions you can ask to determine if something is state?
  Is it passed in as props from a parent? Yes -> NOT STATE
  Does it remain unchanged over time? Yes -> NOT STATE
  Can you compute it using existing state/props? Yes -> NOT STATE
5. How can you identify where state needs to live?
  State shouls live at the lowest component needed to effect changes where you want to.  From the docs:

> 1. Identify every component that renders something based on that state. 
> 2. Find a common owner component (a single component above all the components that need the state in the hierarchy).
> 3. Either the common owner or another component higher up in the hierarchy should own the state.
> 4. If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

## Higher-Order Functions

1. What is a “higher-order function”?
  A higher order function is one that operates on another function wither by taking it in as an argument or by returning it.
2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
  Line 2 returns an arrow function with a single parameter (`m`) and evaluates the expression `m > n`, where `n` is the argument passed into the `greaterThan` function. In this case, it returns `m => m > 10`.
3. Explain how either map or reduce operates, with regards to higher-order functions.
  The map function takes in a callback function as an argument and applies it to each element of the array on which it is called. It returns a new array (of equal length to the initial array) that contains the return values of the callback executed on each element of the initial array.
