# Readings: Redux - Asynchronous Actions
<!-- ### Author -->

## [Async Logic and Data Fetching](https://redux.js.org/tutorials/fundamentals/part-6-async-logic)

### Introduction

React components interact with a Redux store, including calling useSelector to read Redux state, calling useDispatch to give us access to the dispatch function, and wrapping our app in a <Provider> component to give those hooks access to the store.

### Redux Middleware and Side Effects

By itself, a Redux store doesn't know anything about async logic. It only knows how to synchronously dispatch actions, update the state by calling the root reducer function, and notify the UI that something has changed. Any asynchronicity has to happen outside the store.

Earlier, we said that Redux reducers must never contain "side effects". A "side effect" is any change to state or behavior that can be seen outside of returning a value from a function. Some common kinds of side effects are things like:

- Logging a value to the console

- Saving a file

- Setting an async timer

- Making an AJAX HTTP request

- Modifying some state that exists outside of a function, or mutating arguments to a function

- Generating random numbers or unique random IDs (such as Math.random() or Date.now())





















