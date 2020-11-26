# Readings: Context API
<!-- ### Author -->

## [Context](https://reactjs.org/docs/context.html)

Context provides a way to pass data through the component tree without having to pass props down manually at every level.

In a typical React application, data is passed top-down (parent to child) via props, but this can be cumbersome for certain types of props (e.g. locale preference, UI theme) that are required by many components within an application. Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.

### When to Use Context

Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

Using context, we can avoid passing props through intermediate elements.

### Before You Use Context

Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.

If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.

For example, consider a Page component that passes a user and avatarSize prop several levels down so that deeply nested Link and Avatar components can read it.







