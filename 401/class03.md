# Express REST API

## Review, Research, and Discussion

**Name 3 real world use cases where you’d want to change the request with custom middleware**

* Data Management
* Logging Middleware
* Authentcation

**True or false: The route handler is middleware?**

false

**In what ways can a middleware function end the process and send data to the browser?**

using next().

![middleware](https://iq.opengenus.org/content/images/2019/08/Add-a-subheading--2-.png)

**What can cause express to error with “Request headers sent twice, cannot start a second response”**

when you're already in the Body or Finished state, but some function tried to set a header or statusCode. When you see this error, try to look for anything that tries to send a header after some of the body has already been written.




**Vocabulary Terms**

Middleware: Middleware is software that provides common services ,Middleware helps developers build applications more efficiently

Request Object: The request object is the main entry point for an application to issue a request to the Library - all operations on a URL must use a Request object

Response Object:  It is the object which communicates between the server and the output which is sent to the client


Routing Middleware: in Express, usually, we make end-points that uses HTTP verbs to denote a GET POST DELETE PUT etc requests. Router is used to manage these incoming requests.

Test Driven Development: Test Driven Development (TDD) is a software development practice that focuses on creating unit test cases before developing the actual code

Behavioral Testing: is a testing of the external behaviour of the program, also known as black box testing. It is usually a functional testing


## Preview

**Which 3 things had you heard about previously and now have better clarity on?**

* Test Driven Development

**- Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**

* Middleware
* API
* Test Driven Development


**What are you most excited about trying to implement or see how it works?**

Testing

**Review: ES6 Classes**

Classes are a template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes but also have some syntax and semantics that are not shared with ES5 class-like semantics.

Class declarations
One way to define a class is using a class declaration. To declare a class, you use the class keyword with the name of the class

```html

class Rectangle {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
}

```

Hoisting
An important difference between function declarations and class declarations is that function declarations are hoisted and class declarations are not

The body of a class is the part that is in curly brackets {}. This is where you define class members, such as methods or constructor.


**Using Express Routing**

Routing refers to how an application’s endpoints (URIs) respond to client requests.
You define routing using methods of the Express app object that correspond to HTTP methods; for example, app.get() to handle GET requests and app.post to handle POST requests.
These routing methods specify a callback function (sometimes called “handler functions”) called when the application receives a request to the specified route (endpoint) and HTTP method.

**The following code is an example of a very basic route.**

```html

var express = require('express')
var app = express()

// respond with "hello world" when a GET request is made to the homepage
app.get('/', function (req, res) {
  res.send('hello world')
})

```

**Express Routing**

Express 4.0 comes with the new Router. Router is like a mini express application. It doesn't bring in views or settings, but provides us with the routing APIs like .use, .get, .param, and route.

* Basic Routes:  express.Router()

* Route Middleware :router.use() Route middleware in Express is a way to do something before a request is processed.

* Route with Parameters like  /hello/:name

* Route Middleware for Parameters to validate specific parameters, We will use Express's .param() middleware. This creates middleware that will run for a certain route parameter.

* Login routes Doing a GET and POST on /login
Validates a parameter passed to a certain route, We can define our routes right on our app. This is similar to using app.get, but we will use app.route. app.route is basically a shortcut to call the Express Router. Instead of calling express.Router(), we can call app.route and start applying our routes there.





