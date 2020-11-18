# Readings: Props and State
<!-- ### Author -->

## Review, Research, and Discussion

- Does a deployed React application require a server?

  - You don’t necessarily need a static server in order to run a Create React App project in production. It also works well when integrated into an existing server side app.

  (https://create-react-app.dev/docs/deployment/)

- Why do we prefer to test a React application at the behavior rather than the unit level?

  - Focusing on testing users behavior rather than the implementation allows you to easily refactor code going forward. You want your user experience to be the same regardless of your implementation details…

  (https://medium.com/@boyney123/my-experience-moving-from-enzyme-to-react-testing-library-5ac65d992ce)

- What does npm run build do?

  - npm run build creates a build directory with a production build of your app. Set up your favorite HTTP server so that a visitor to your site is served index.html, and requests to static paths like /static/js/main.<hash>.js are served with the contents of the /static/js/main.<hash>.js file.

  (https://create-react-app.dev/docs/deployment/)


- Describe the actual composition / architecture of a React application

  - The key feature of React is composition of components. Components written by different people should work well together. It is important to us that you can add functionality to a component without causing rippling changes throughout the codebase.

  - For example, it should be possible to introduce some local state into a component without changing any of the components using it. Similarly, it should be possible to add some initialization and teardown code to any component when necessary.