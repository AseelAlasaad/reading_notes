# Reading: Context API

# Review, Research, and Discussion

* Describe use cases useState() vs useReducer()?

  The useState function is a built in hook that can be imported from the react package. It allows you to add state to your functional components. Using the useState hook inside a function component

  UseReducer is a React hook function that accepts a reducer function, and an initial state

* Why do custom hooks need the use prefix?

  Custom Hook is a JavaScript function which we create by ourselves, when we want to share logic between other JavaScript functions. It allows you to reuse some piece of code in several parts of your app

* What do custom hooks usually do?

    Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.


# Term

* reducer: A reducer is a function that determines changes to an application's state

# Preview


* Which 3 things had you heard about previously and now have better clarity on?

   Hooks, useState, useReducer
* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

  Hooks, useState, useReducer

* What are you most excited about trying to implement or see how it works?
  
  Hooks, useState, useReducer

# Preparation Materials

**Context**

Context provides a way to pass data through the component tree without having to pass props down manually at every level.

**Use Context**

Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. For example, in the code below we manually thread through a “theme” prop in order to style the Button component: