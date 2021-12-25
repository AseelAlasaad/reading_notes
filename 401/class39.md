# Readings: Redux - Additional Topics

# Review, Research, and Discussion


* What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?

    The most 'redux-like' way of handling the pre-loading of data would be to fire off the asynchronous action in the lifecycle method

* When using a thunk/async action that dispatches the actual action, which do you export from your reducer?

        
    To dispatch async actions into our store, we have to apply the thunk middleware by writing: const store = createStore(joke, applyMiddleware(thunk)); to apply the middleware. Then in App , we call dispatch with the function returned from the fetchJoke passed inside

# Term
* middleware: llows for side effects to be run without blocking state updates. We can run side effects (like API requests) in response to a specific action, or in response to every action that is dispatched (like logging).
* thunk:Thunk is middleware that allows you to return functions, rather than just actions, within Redux

# Preview

* Which 3 things had you heard about previously and now have better clarity on?
 
  Redux
* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

    Redux
* What are you most excited about trying to implement or see how it works?

    Redux

# Preparation Materials


The Redux Toolkit package is intended to be the standard way to write Redux logic. It was originally created to help address three common concerns about Redux:

"Configuring a Redux store is too complicated"
"I have to add a lot of packages to get Redux to do anything useful"
"Redux requires too much boilerplate code"

# Installation​

**Using Create React App**

**npx create-react-app my-app --template redux**

**An Existing App​**

Redux Toolkit is available as a package on NPM for use with a module bundler or in a Node application:

# NPM
npm install @reduxjs/toolkit

[Redux Toolkit](https://redux-toolkit.js.org/introduction/getting-started)