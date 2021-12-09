# Reading: useState() Hook

# Review, Research, and Discussion

* How does React differ from vanilla JS/HTML/CSS?

React JS is a JavaScript library for single page applications. React also allows us to create reusable components. React allows developers to create large web applications that can change data, without reloading the page. The main purpose of React is to be fast, scalable, and simple. It works only on user interfaces in the application.

The component-based approach, well-defined lifecycle, and use of just plain JavaScript make React very simple to learn, build a professional web (and mobile applications), and support it. React uses a special syntax called JSX which allows you to mix HTML with JavaScript. This is not a requirement; Developer can still write in plain JavaScript but JSX is much easier to use.

VanillaJS is a name to refer to using plain JavaScript without any additional libraries like jQuery

* What is the primary difference between a function component and a class component?

A functional component is just a plain JavaScript function that accepts props as an argument and returns a React element. A class component requires you to extend from React. Component and create a render function which returns a React element. There is no render method used in functional components.

# Term
 
* Functional Components : are basic JavaScript functions. These are typically arrow functions but can also be created with the regular function keyword. Functional components are functions that takes in props and return JSX.

* Children / Child Components:Children allow you to pass components as data to other components

# Preview

* Which 3 things had you heard about previously and now have better clarity on?

   React

* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   
   Hooks

* What are you most excited about trying to implement or see how it works?

   React, Hooks, useState

# Preparation Materials

**Using the State Hook**

Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class

```html

import React, { useState } from 'react';

function Example() {
  // Declare a new state variable, which we'll call "count"
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}

```

**What is a Hook?**

 A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components.

**What does useState return?**

 It returns a pair of values: the current state and a function that updates it. This is why we write const [count, setCount] = useState(). This is similar to this.state.count and this.setState in a class.

 ```html

 const [count, setCount] = useState(0);

 ```
