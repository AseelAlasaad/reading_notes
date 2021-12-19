# Reading: Application State with Redux

# Review, Research, and Discussion

* What are the advantages of storing tokens in “Cookies” vs “Local Storage”
        easier to retrive and edit.

        easier to clean or reset.

        cookies data will be sent over each request which is great to authentication and authorization.
    
* Explain 3rd party cookies.
        Third-party cookies work by embedding JavaScript from one website into another. Third-party cookies store data remembered between browsing sessions
* How do pixel tags work?

        pixel tag) is a graphic with dimensions of 1x1 pixels that is loaded when a user visits a webpage 

# Term

* cookies : are files created by websites you visit. They make your online experience easier by saving browsing information
* authorization : is a process by which a server determines if the client has permission to use a resource or access a file
* access control : is the mechanism by which access to web pages is limited to specific users
* conditional rendering :  is a term to describe the ability to render different user interface (UI) markup if a condition is true or false.


# Preview


* Which 3 things had you heard about previously and now have better clarity on?
   cookies
* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    Redux
* What are you most excited about trying to implement or see how it works?
   Redux


# Preparation Materials

**Redux**

Redux is a predictable state container for JavaScript apps

It helps you write applications that behave consistently, run in different environments (client, server, and native), and are easy to test


Redux is used mostly for application state management. To summarize it, Redux maintains the state of an entire application in a single immutable state tree (object), which can't be changed directly.

* The createStore factory function from Redux is used to create a Redux STORE.
* The Reducer is the only mandatory argument passed into createStore()
* A REDUCER is just a function. A function that takes in two parameters. The first is the STATE of the app, and the other is an ACTION.
* A Reducer always returns the new stateof your application.