# Readings: Component Composition
<!-- ### Author -->

## Review, Research, and Discussion

Can a parent component access the state of a child component?

- Yes, by using a callback function. The most common method is to make a callback function that the child component will trigger and toss the state values upward.

What can be passed along in a prop variable?

- string, integers, object, arrays


How can a child component “know” the state of another component?

- By passing the state of a component to another component as props