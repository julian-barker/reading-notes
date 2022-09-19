[Home](../README.md)

# Class 01

## Initital Questions

### What is React?

React is a user-interface (UI) library. It has a component architecture, one-way data flow, and component state.

### What is a component?

A component is a small piece of a site.

### What is the dataflow of React?

It's the passing of state data from one component to another.

### How do we make a React element a DOM element?

Pass it through react-DOM library with the .render() method.

### React is a User Interface ______.

React is a User Interface library. This means that it will be used to create user interfaces for sites.

### Which direction does data flow in React?

Data flows down one way through an app.

### Every component manages its own ____.

Every component manages its own state.

## Component-based Architecture

- Component-based architecture breaks up design into smaller functional or logical pieces (components)
- The primary objective is to ensure component reusability
- A component is a modular, portable, replaceable, and reusable set of functionality that encapsulates its implementation
- Component views:
  - Object-oriented view - a component is a set of two or more cooperating classes
  - Conventional view - a component is a functional element that icorporates the processes, data structures, and interface required to use it
  - Process-related view - as opposed to creating components, the system leverages existing components from libraries

- Component Characteristics:
  - reusable
  - replaceable
  - not context-specific
  - extensible
  - encapsulated
  - independent

- Component Advantages:
  - ease of deployment
  - reduced cost
  - ease of development
  - reusable
  - modification of technical complexity
  - reliability
  - system maintenance and evolution
  - independent

### Takeaways

- Seems like a bad marketing pitch to me...

## Props

- Props is short for properties and refers to properties of a component
- Props are used to pass data from parent to child components
- The flow of data in props is one-way and only travels down the hierarchy (parent -> child)
