# Reading: Component Lifecycle / useEffect() Hook

# Review, Research, and Discussion

* Why do we not need more .html pages in a multi-page React app?
   
   React is not designed to develop multi-page websites. So, we need to create multiple routes to handle multiple views

* If we wanted a component to show up on every page, where would we put it and why?

  Inside the <BrowserRouter />, outside a <Route />



* What does routing do with the components that were rendered when a new route is requested?
  
  it goes to the new componetnt and remove the old one clean ups

* What does props.children contain?

  props. children does is that it is used to display whatever you include between the opening and closing tags when invoking a component

* How do useState() and this.setState() differ?

  SetState() does not immediately mutate this. state but creates a pending state transition. Accessing this. state after calling this method can potentially return the existing value



# Term

* State Hook: A Hook is a special function that lets you “hook into” React features

* Mounting and Un-Mounting: The main job of React is to figure out how to modify the DOM to match what the components want to be rendered on the screen. React does so by "mounting" (adding nodes to the DOM), "unmounting" (removing them from the DOM)

# Preview

Which 3 things had you heard about previously and now have better clarity on?

Hooks.

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

useEffect Hook.

What are you most excited about trying to implement or see how it works?

Hooks.

# Preparation Materials

**effects hook**

By using this Hook, you tell React that your component needs to do something after render. React will remember the function you passed (we’ll refer to it as our “effect”), and call it later after performing the DOM updates. In this effect, we set the document title, but we could also perform data fetching or call some other imperative API.

```html


import React, { useState, useEffect } from 'react';

function Example() {
  const [count, setCount] = useState(0);

  useEffect(() => {
    document.title = `You clicked ${count} times`;
  });

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
