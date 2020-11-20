# Readings: Routing
<!-- ### Author -->

## Review, Research, and Discussion

- Do child components have direct access to props/state from the parent?

  - We can see there is no way to pass props from a child component to a parent component. However, we can always pass around functions from the parent to child component. The child component can then make use of these functions.

  (https://www.pluralsight.com/guides/how-to-pass-props-object-from-child-component-to-parent-component)


- When a component “wraps” another component, how does the child component’s output get rendered?

    - The wrapped component receives all the props of the container, along with a new prop, data, which it uses to render its output. The HOC isn’t concerned with how or why the data is used, and the wrapped component isn’t concerned with where the data came from.


- Can a component, such as `<Content />`, which is a child also be used as a standalone component elsewhere in the application?

  - it really depends on your React application on whether you want to use the generic Form component (e.g. Form) or specialize it as standalone Form component with a special use case 

- What trick can a parent use to share all props with it’s children

  - You can do so with the spread operator. This syntax is much easier to the eye, much less error prone, and it allows flexibility, since you don’t need to change the props names or add props in the intermediate component when you change them.

