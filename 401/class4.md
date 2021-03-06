# Review, Research, and Discussion

**Name 3 advantages to Test Driven Development**

Easier to refactor
High test coverage
Easier to maintain

**In what case would you need to use beforeEach() or afterEach() in a test suite?**

The difference is beforeEach()/afterEach() automatically run before and after each tests, which 1. removes the explicit calls from the tests themselves, and 2. ... Tests should be explicit, and tests should never share state.

**What is one downside of Test Driven Development**

TDD is Time Consuming and Costly, in both Short Term and Long Term. In previous section we've already discussed why TDD is time consuming in short term: you have to spend significant time on refactoring and rewriting your code. But in the long term it will cost more time as well

**What’s the primary difference between ES6 Classes and Constructor/Prototype Classes**?

ES5 function constructors :this also uses a new operator for object creation but focuses on how the objects are being instantiated

ES6 class constructors: This can be said to be a syntax base for constructor functions and instantiate objects using a new operato

**Why REST?**

REST stands for Representational State Transfer. It's an architectural pattern for creating web services. A RESTful service is one that implements that pattern.REST can handle multiple types of calls, return different data formats and even change structurally with the correct implementation of hypermedia


## Vocabulary Terms

functional programming: is a programming paradigm where programs are constructed by applying and composing functions.

object-oriented programming (OOP): is based on the concept of objects. In object-oriented programming data structures, or objects are defined, each with its own properties or attributes. Each object can also contain its own procedures or methods. Software is designed by using objects that interact with one another

Class: a class describes the contents of the objects that belong to it.

super: The super keyword is used to access and call functions on an object's parent

this: The this keyword refers to the current object in a method or constructor. this refers to the global object.

TDD: Test Driven Development (TDD) is software development approach in which test cases are developed to specify and validate what the code will do.

jest: Jest is an open-source testing framework built on JavaScript.

Continuous Integration (CI): CI is a modern software development practice in which incremental code changes are made frequently and reliably.

Data Model: data model (or datamodel) is an abstract model that organizes elements of data

**Which 3 things had you heard about previously and now have better clarity on?**

OOP 
Class 
this

**Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**

Data model

sequelize

**What are you most excited about trying to implement or see how it works?**

TDD

Data Model

## Preview

**nosql vs sql**

SQL databases are primarily called as Relational Databases (RDBMS); whereas NoSQL database are primarily called as non-relational or distributed database.

SQL databases are table based databases whereas NoSQL databases are document based, key-value pairs, graph databases or wide-column stores. This means that SQL databases represent data in form of tables which consists of n number of rows of data whereas NoSQL databases are the collection of key-value pair, documents, graph databases or wide-column stores which do not have standard schema definitions which it needs to adhered to.

SQL databases have predefined schema whereas NoSQL databases have dynamic schema for unstructured data.


**sequelize api**

Sequelize is a promise-based Node.js ORM tool for Postgres, MySQL, MariaDB, SQLite and Microsoft SQL Server. 

