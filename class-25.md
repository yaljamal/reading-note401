# Hooks API

Hooks are JavaScript functions its lets you use state and other features in React without writing a class.

## roles for Hooks

1. Hooks must be named with a `use` prefix (i.e. `useFishingPole` )
2. Only call Hooks at the top level. Don’t call Hooks inside loops, conditions, or nested functions.
3. Only call Hooks from React function components. Don’t call Hooks from regular JavaScript functions

* there is a build in Hooks

> `useState()` Returns a stateVariable and setterFunction for you to use to manage state in a functional component

 EX : 
`clicks` is the state variable, which will store the number of clicks

`setClicks` is a function that is called to change the value of clicks 

## Effect Hook

It serves the same purpose as componentDidMount, componentDidUpdate, and componentWillUnmount it will serve after every render include the first render
