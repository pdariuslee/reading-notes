# Readings: Redux - Additional Topics
<!-- ### Author -->

## [Redux Toolkit](https://redux-toolkit.js.org/)

**Simple**

Includes utilities to simplify common use cases like store setup, creating reducers, immutable update logic, and more.

**Opinionated**

Provides good defaults for store setup out of the box, and includes the most commonly used Redux addons built-in.

**Powerful**

Takes inspiration from libraries like Immer and Autodux to let you write "mutative" immutable update logic, and even create entire "slices" of state automatically.

**Effective**

Lets you focus on the core logic your app needs, so you can do more work with less code.

### Purpose

The Redux Toolkit package is intended to be the standard way to write Redux logic. It was originally created to help address three common concerns about Redux:

- "Configuring a Redux store is too complicated"

- "I have to add a lot of packages to get Redux to do anything useful"

- "Redux requires too much boilerplate code"

We can't solve every use case, but in the spirit of create-react-app and apollo-boost, we can try to provide some tools that abstract over the setup process and handle the most common use cases, as well as include some useful utilities that will let the user simplify their application code.

Because of that, this package is deliberately limited in scope. It does not address concepts like "reusable encapsulated Redux modules", data caching, folder or file structures, managing entity relationships in the store, and so on.

That said, these tools should be beneficial to all Redux users. Whether you're a brand new Redux user setting up your first project, or an experienced user who wants to simplify an existing application, Redux Toolkit can help you make your Redux code better.

What's Included

Redux Toolkit includes these APIs:

configureStore(): wraps createStore to provide simplified configuration options and good defaults. It can automatically combine your slice reducers, adds whatever Redux middleware you supply, includes redux-thunk by default, and enables use of the Redux DevTools Extension.

createReducer(): that lets you supply a lookup table of action types to case reducer functions, rather than writing switch statements. In addition, it automatically uses the immer library to let you write simpler immutable updates with normal mutative code, like state.todos[3].completed = true.

createAction(): generates an action creator function for the given action type string. The function itself has toString() defined, so that it can be used in place of the type constant.

createSlice(): accepts an object of reducer functions, a slice name, and an initial state value, and automatically generates a slice reducer with corresponding action creators and action types.

createAsyncThunk: accepts an action type string and a function that returns a promise, and generates a thunk that dispatches pending/fulfilled/rejected action types based on that promise

createEntityAdapter: generates a set of reusable reducers and selectors to manage normalized data in the store

The createSelector utility from the Reselect library, re-exported for ease of use.