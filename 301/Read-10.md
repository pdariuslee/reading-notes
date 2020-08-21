# The Call Stack and Debugging

## [Call stack](https://developer.mozilla.org/en-US/docs/Glossary/Call_stack)

### From developer.mozilla.org


- Call stack

  - A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.

    - When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.

    - Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.

    - When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.

    - If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.

    - In summary, then, we start with an empty Call Stack. Whenever we invoke a function, it is automatically added to the Call Stack. Once the function has executed all of its code, it is automatically removed from the Call Stack. Ultimately, the Stack is empty again.


 ---


 ## [The JavaScript Call Stack - What It Is and Why It's Necessary](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)

 ### By Charles Freeborn

 - The **call stack** is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is **synchronous**.


- In Asynchronous JavaScript, we have a callback function, an event loop, and a task queue. The callback function is acted upon by the call stack during execution after the call back function has been pushed to the stack by the event loop.

- In summary

  - It is single-threaded. Meaning it can only do one thing at a time.

  - Code execution is synchronous.

  - A function invocation creates a stack frame that occupies a temporary memory.
  
  - It works as a LIFO — Last In, First Out data structure.



 ---


 ## [JavaScript error messages && debugging](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

 ### By Diogo Spinola

  - Types of error messages

    - Reference errors

    - Syntax errors

    - Range errors

    - Type errors

- Debugging

  - To **debug** your JS code, the **easiest** and maybe the most common way its to simply **console.log()** the variables you want to check or, by **using chrome developer tools**, open your page with your JS code (press cmd+o in macOS or Ctrl+o in Windows) and choose your file to debug, click the line you wanna debug and refresh your page again (F5)

  - The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.

  - You can also add conditional breakpoints by right-clicking a previous set breakpoint, which will make your program stop at that point only if a condition is met, this is awesome for when you want to debug huge cycles for specific values. In this example the breakpoint will point stop when the index reaches 40.

- Handling errors

  - To avoid this we usually try to catch the errors so we can gracefully fallback to a default state of our application in case of an error (this fallback can be a 404 page which is normally not that graceful but is better than a page to just stop working).

- An alternative it’s to encapsulate our problematic function code with a **try…catch** which would make an error be thrown but this time, not “uncaught” so we can send it to a error logging to be checked later and send a fallback to the function so that our code continues without problems.



---

[Back to Home](https://pdariuslee.github.io/reading-notes/)