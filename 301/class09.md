# Concepts of Functional Programming in Javascript

**What is functional programming?**
Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data 

**What is a pure function and how do we know if something is a pure function?**

The definition of a pure function is: The function always returns the same result if the same arguments are passed in. It does not depend on any state, or data, change during a program's execution. It must only depend on its input arguments.

**What are the benefits of a pure function?**


One of the major benefits of using pure functions is they are immediately testable. They will always produce the same result if you pass in the same arguments. They also makes maintaining and refactoring code much easier..

**What is immutability?**

Unchanging over time or unable to be changed.When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

**What is Referential transparency?**


Referential transparency and referential opacity are properties of parts of computer programs.  An expression is called referentially transparent if it can be replaced with its corresponding value (and vice-versa) without changing the program's behavior