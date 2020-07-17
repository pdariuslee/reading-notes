# From the Duckett JS book

## Chapter 10: "Error Handling & Debugging / JS Debugging"

- If you understand execution contexts (which have two stages) and stacks, you are more likely to find the rror in your code.

- Debugging is the proess of finding erros. It involves a process of deduction.

- The console helps narrow down the area in which the error is located, so you can try to find the exact error.

- JS has 7 different types of errors. Each creates its own error object, which can tell you its line number and gives a description of the error.

- If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements. Use them to give your users helpful feedback.

- Error Objects

  - When an error object is created, it will contain the following properties:
  
    - name - type of error
    
    - message - Description
    
    - file number - Name of the JS file
    
    - lineNumber - Line number of error
    
  - 7 types of built-in error objects in JS.
  
    - Error
    
    - SyntaxError
    
    - Reference Error
    
    - Type Error
    
    - Range Error
    
    - URIError
    
    - EvalError

 




 

[Back to Home](https://pdariuslee.github.io/reading-notes/)
