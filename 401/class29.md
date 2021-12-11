# Reading: Advanced State with Reducers

# Review, Research, and Discussion


How can we ensure that an effect hook runs only once?

  
  If you only want to run the function given to useEffect after the initial render, you can give it an empty array as second argument

Can useState() update more than one state variable at the same time?

  ou could combine the loading state and data state into one state object and then you could do one setState call and there will only be one render. Note: Unlike the setState in class components, the setState returned from useState doesn't merge objects with existing state, it replaces the object entirely.

Is useState() synchronous?

 useState and setState both are asynchronous.



# Term

* State Hook: useState is a Hook that allows you to have state variables in functional components.

* Component Lifecycle : in React has a lifecycle which you can monitor and manipulate during its three main phases. The three phases are: Mounting, Updating, and Unmounting


# Preview

* Which 3 things had you heard about previously and now have better clarity on?

  Hooks, useState, useEffect
* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
 
  Hooks, useState, useEffect

* What are you most excited about trying to implement or see how it works?

  Hooks, useState, useEffect


# Preparation Materials

**useReducer hook**

An alternative to useState. Accepts a reducer of type (state, action) => newState, and returns the current state paired with a dispatch method.

useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components

```html 

const [state, dispatch] = useReducer(reducer, initialArg);
```