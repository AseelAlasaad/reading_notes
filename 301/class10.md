# The JavaScript Call Stack

![stack](https://cdn-media-1.freecodecamp.org/images/QgR2uIk7tW0YNz0Xm8g0jAPeRFI0e4sCejsv)

**What is a ‘call’?**

The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.a call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).




**What does LIFO mean?**

LIFO: When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.


 It works as a LIFO — Last In, First Out data structure.

![stack](https://www.codeproject.com/KB/mcpp/5256936/stack.png)

**What causes a Stack Overflow?**

A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

## JavaScript error messages

![error](https://miro.medium.com/max/1000/1*LHpmsxV3f2znpxhuAFuIqA.png)

**What is a ‘refrence error’?**

This is also a common thing when using const and let, they are hoisted like var and function but there is a time between the hoisting and being declared so when you try to access them a reference error occurs, the fact that this happens to let and const is called Temporal Dead Zone (TDZ).


**What is a ‘syntax error’?**

this occurs when you have something that cannot be parsed in terms of syntax.

**What is a ‘range error’?**

A RangeError is thrown when trying to pass a number as an argument to a function that does not allow a range that includes that number. This can be encountered when to create an array of an illegal length with the Array constructor

**What is a ‘tyep error’?**

this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.This is probably the most frequent error in JS

**What is a breakpoint?**

 A breakpoint is a point in the program where the code will stop executing

