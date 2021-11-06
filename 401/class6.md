# Review, Research, and Discussion

**Explain what a “Singleton” is (in Computer Science terms)**


A singleton is a class that allows only a single  instance of itself to be created and gives access to that created instance .It contains static variables that can accommodate unique and private instances of itself.The singleton pattern is used in programming languages.The Singleton's purpose is to control object creation.

**Explain how the Singleton pattern can be used with Node modules, specifically with classes.**

Creating singleton in Node.JS is very easy. We need singleton when we want to make sure there is only one object instantiated. Therefore, instead of creating a new object we need to ensure the constructor was called only once and then we reuse the instance.

We can achieve this by refactoring our class to have:

* hidden (private)constructor
* public getInstance method that returns instance of the class

Sometimes you need to make sure that you have one and only one instance of an object. This is where the singleton pattern can be useful. A singleton represents a single instance of an object. Only one can be created, no matter how many times the object is instantiated. If there’s already an instance, the singleton will create a new one. Let’s take a look at where creating multiple instances of one object might create problems within our application.A singleton represents a single instance of an object. Only one can be created, no matter how many times the object is instantiated. If there's already an instance, the singleton will create a new one


# Term

* Router Middleware : 
Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application's request-response cycle

* Dynamic Module Loading : 
Dynamic loading is a mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory

* Singleton Pattern: define a class that has only one instance and provides

* CRUD -> REST Method Matches : CRUD stands for Create, Read, Update, and Delete.CRUD principles are mapped to REST commands to comply with the goals of RESTful architecture.REST stands for representational state transfer 

* Mock Testing: The Full Form of MOCK is Multiple option checking


# Preview
**Which 3 things had you heard about previously and now have better clarity on?**
CRUD -> REST Method Matches

**Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**

Singleton Pattern

Mock Testing 

Dynamic Module Loading

**What are you most excited about trying to implement or see how it works?**

Mock Testing

**Securing Passwords**

Passwords are the first line of defense against cyber criminals. It is the most vital secret of every activity we do over the internet and also a final check to get into any of your user account, whether it is your bank account, email account, shopping cart account or any other account you have.

We all know storing passwords in clear text in your database is ridiculous. Many desktop applications and almost every web service including, blogs, forums eventually need to store a collection of user data and the passwords, that has to be stored using a hashing algorithm.

Cryptographic hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3 are general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible.Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.

**Basic Auth**


In the context of an HTTP transaction, basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request.

HTTP Basic authentication (BA) implementation is the simplest technique for enforcing access controls to web resources because it does not require cookies, session identifiers, or login pages; rather, HTTP Basic authentication uses standard fields in the HTTP header.

**OWASP auth cheatsheet**

Authentication is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

Session Management is a process by which a server maintains the state of an entity interacting with it. This is required for a server to remember how to react to subsequent requests throughout a transaction.

User IDs

Make sure your usernames/user IDs are case-insensitive. User 'smith' and user 'Smith' should be the same user. Usernames should also be unique. For high-security applications, usernames could be assigned and secret instead of user-defined public data.

Password Length
Minimum length of the passwords should be enforced by the application. Passwords shorter than 8 characters

**bcrypt docs**

A library to help you hash passwords,
The bcrypt hashing function allows us to build a password security platform that scales with computation power and always hashes every password with a salt


