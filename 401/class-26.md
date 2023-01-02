[Home](../README.md)

# Class 26

## Component-Based UI

- Components are the building blocks of a React app.
- An element is a native component of HTML and is what the DOM is made of.
- A react component is a reuseable encapsulated piece of code that produces a representation of a set of HTML elements. It can be static, always returning the same thing, or dynamic, and change based on input or its surroundings.
- React's component based architecture allows heavy reusability of code, and separates concerns in a potentially more logical manner than the typical language-based separation of concerns used in a vanilla HTML, JS, and CSS app.

### JSX

- JSX is javascript that produces valid HTML. It allows developers to effectively write HTML dynamically.
- To embed JS expressions in JSX, surround the expression with curly braces and the implicit or explicit return value of the expression will be inserted into the JSX at that position.
- It is safe to embed user input into JSX with react as it is sterilized and converted to pure string form by React DOM. This prevents XSS attacks.

### Rendering

- A react component is a reusable piece of code that contains everything about a distinct portion of an application, from its appearance to its behavior.
- React components are immutable, meaning that they cannot change once they are rendered. To change something inside a rendered component, we re-render that component and everything inside it.
- When the UI changes, only that specific portion of the UI actually gets changed in the DOM, though the entire component containing that piece of UI is re-rendered. This happens through recreating the virtual DOM and comparing it to the real DOM.
  - While this is computationaly cheaper than recreating the DOM on every re-render, there is still some overhead in re-rendering the component, updating the VDOM, and comparing the changes to the DOM.
