# Error Handling & Debugging

Errors, bugs, and therefore debugging are a part of life for a programmer,Dealing with errors actually involves two very different processes: error handling and debugging.

 Error Handling and Debugging. ... Error handling is a combination of coding and methodology that allows your program to anticipate user and other errors. It allows you to create a robust program.

If you encounter a problem with your code, there are a number of methods available to help you track it down. 

    * THE CONSOLE & DEV TOOLS
        Tools built into the browser
        that help you hunt for errors

    * COMMON PROBLEMS

        Common sources of errors,
        and how to solve them

    * HANDLING ERRORS
    
       How code can deal with potential errors gracefully 

To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run.

    **EXECUTION CONTEXT**
    *  GLOBAL CONTEXT
    * FUNCTION CONTEXT
    * EVAL CONTEXT (NOT SHOWN)

**UNDERSTANDING ERRORS**

    If a JavaScript statement generates an error, then it throws an exception.
    At that point, the interpreter stops and looks for exception-handling code.

    When an exception is thrown, the interpreter
    stops and checks the current execution context for
    exception-handling code.

**ERROR OBJECTS**

    Error objects can help you find where your mistakes are and browsers have tools to help you read them.

    When an Er ror object is created, it will contain the following properties:


    name : Type of execution

    message : Description

    fil eNumber :Name of the JavaScript file

    lineNumber :Line number of error

    There are seven types of built-in error objects in
    JavaScript such as Syntax Error,TypeError,Ref erenceError.

![error](https://infoheap.com/wp-content/uploads/2016/03/chrome-developer-tools-console-javascript-errors.png)

**HOW TO DEAL WITH
ERRORS**

Now that you know what an error is and how the browser treats them,
there are two things you can do with the errors.

1. DEBUG THE SCRIPT TO FIX ERRORS
    
    If you come across an error while writing a script
    , you will need to debug the code, track down the source of the error,
    and fix it

2. HANDLE ERRORS GRACEFULLY

    You can handle errors gracefully using try, catch,
    throw, and f i na 1 ly statement s.

Debugging is the process of finding errors. It involves a
process of deduction.

The console helps narrow down the area in which the
error is located, so you can try to find the exact error

![trycatch](https://res.cloudinary.com/practicaldev/image/fetch/s--KOQ2vBoR--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/i/3ufdubowaga0tdehgdin.jpeg)

