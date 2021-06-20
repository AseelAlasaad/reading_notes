# Function 


![function](https://learncodeweb.com/wp-content/uploads/2020/06/How-to-define-and-call-a-function-in-JavaScript-with-example.png)


A JavaScript function is a block of code designed to perform a particular task,functions allow a programmer to divide a big program into a number of small and manageable functions. Before we use a function, we need to define it.

## Function Definition

The most common way to define a function in JavaScript is by using the function keyworda ,list of parameters (that might be empty), and a statement block surrounded by curly braces.

Syntax:

![syntax](https://cdn.programiz.com/cdn/farfuture/oAZVf3IqOKOYj_aJ-IoYQvbJ2CB-B3y4HXSLXBUmYcY/mtime:1591592163/sites/tutorial2program/files/javascript-function-with-parameter.png)

There are two way to defining functions:

* Function declarations
 
 function functionName(parameters) {
  // code to be executed
}




* Function expressions

var foo = function() { //code to be executed }

The code inside a function is executed when the function is invoked,look at of this example about how invoke the function:

function myFunction(a, b) {
  return a * b;
}
myFunction(10, 2); //calling function.
