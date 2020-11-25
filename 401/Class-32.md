# Readings: Custom Hooks
<!-- ### Author -->

## React Hooks

useEffect Hook

- use it without cleanup
- with cleanup.

useEffect tells React that our component needs to do something after the component renders. It runs after the first render and after every update.

Below is an example of how useEffect can run without any cleanup:

  useEffect(() => {

      document.title = `You clicked ${count} times`;
          });

If you do need cleanup to run, you can return a function from useEffect. This is optional and it allows you to run some code after your effect and before any new effect runs. A situation where you subscribe to something may need an unsubscribe as part of the effects cleanup process. React will perform this cleanup on unmount.

useEffect(() => {

      console.log("Subscribe to Something);

      return function cleanup() {

        console.log("Unsubscribe to Something);
      };
    });

The effect above will run on every render more than one time. React cleans up effects from the previous render before running the effects of the next render, and this should be noted.