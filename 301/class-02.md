[Home](../README.md)

# Class 02

## Reading

- Mounting, Updating, and Unmounting are the three phases of a React component's lifecycle
- Mounting phase is when a component gets created and inserted into the DOM
  - The following lifecycle events happen in the mounting phase in the following order:
    - static `getDerivedStateFromProps`, `render`, `componentDidMount`, and `UNSAFE_componentWillMount`
  - Additionally, the constructor function executes in the mounting phase
- Updating phase is when a component is in the DOM. During this phase, a component can be updated or undergo state changes
  - The following lifecycle events happen in the updating phase in the following order:
    - static `getDerivedStateFromProps`, `shouldComponentUpdate`, `render`,
`getSnapshotBeforeUpdate`, `componentDidUpdate`, `UNSAFE_componentWillUpdate`, `UNSAFE_componentWillReceiveProps`
- Unmounting phase is when a component is being removed from the DOM
  - The only lifecycle event in the mounting phase is `componentWillUnmount`
- `render()` - the only required method in a class component, and should not modify `this.state`
- `componentDidMount()` - this method is called after the component mounts
- `shouldComponentUpdate()` - by default, react rerenders after every update. If this method is set to `false`, then `UNSAFE_componentWillUpdate()`, `render()`, and `componentDidUpdate()` will not be called
- `componentDidUpdate()` - useful for performing network requests after a componenet updates
- `componentWillUnmount()` - this method is used to clean up the DOM and subscriptions

1. render() happens before componentDidMount()
2. The very first action in React is the calling of a component's constructor function
3. constructor -> render -> React Updates -> componentDidMount -> componentWillUnmount
4. componentDidMount executes a specified set of instructions as soon as the component is mounted

## Video

1. Props are like arguments to a function - you can pass anything into a component's props (primitives, objects, functions, etc.)
2. Props are passed into a component and state resides and is handled within a component
3. We rerender any time state is changed within a component
4. State is useful for things such as a counter that may change based on events or over time, and affect the way a component looks or behaves. State is used for data that will never be used by any component higher than the component it resides in
