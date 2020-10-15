# Readings: Data Modeling & NoSQL Database

1. Name 3 advantages to Test Driven Development
    
    - Better program design and higher code quality

    - Detailed project documentation

    - TDD reduces the time required for project development

    (https://www.codica.com/blog/test-driven-development-benefits/)

2. In what case would you need to use beforeEach() or afterEach() in a test suite?

    - The **beforeEach** function executes before any spec in the describe block containing it, as well as before any spec contained inside any inner describe. The **afterEach** are used for whatever cleanup is needed at the conclusion of the specs, and are not covered as part of this document.

    (http://breazeal.com/blog/jasmineBefore.html)

3. What is one downside of Test Driven Development

    - It necessitates a lot of time and effort up front, which can make development feel slow to begin with.

    (https://leantesting.com/test-driven-development/)

4. What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?

  - a class defines a type which can be instantiated at runtime, whereas a prototype is itself an object instance.

    (https://www.toptal.com/javascript/es6-class-chaos-keeps-js-developer-up#:~:text=A%20child%20of%20an%20ES6,t%20implemented%20on%20the%20child.)

5. Name a use case for a static method

  - The code in the method is not dependent on instance creation and is not using any instance variable.

    (https://www.tutorialspoint.com/When-to-use-static-methods-in-Java)

6. Write an example of a Higher Order function and describe the use case it solves

  - Example: Array.prototype.map

  - The map() method creates a new array by calling the callback function provided as an argument on every element in the input array. The map() method will take every returned value from the callback function and creates a new array using those values.
The callback function passed to the map() method accepts 3 arguments: element, index, and array.

    (https://blog.bitsrc.io/understanding-higher-order-functions-in-javascript-75461803bad)


[Back to Home](https://pdariuslee.github.io/reading-notes/)