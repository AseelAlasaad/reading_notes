# React


**What is React?**

React is a declarative, efficient, and flexible JavaScript library for building user interfaces. It lets you compose complex UIs from small and isolated pieces of code called “components”. react. js is an open-source JavaScript library that is used for building user interfaces specifically for single-page applications. It's used for handling the view layer for web and mobile apps.React.js is the most popular front-end JavaScript library for building Web applications.React allows developers to create large web applications that can change data, without reloading the page. The main purpose of React is to be fast, scalable, and simple.

![reac](https://csharpcorner-mindcrackerinc.netdna-ssl.com/article/what-and-why-reactjs/Images/image005.jpg)

**What is a component?**

Components are the building blocks of any React application, and a single app usually consists of multiple components. A component is essentially a piece of the user interface. React splits the UI into independent, reusable parts that can be processed separately.


![react](https://www.simplilearn.com/ice9/free_resources_article_thumb/model-view.JPG)

There are two types of components in React:

* Functional Components :  These components have no state of their own and only contain a render method, so they are also called stateless components. They may derive data from other components as props (properties).

* Class Components : These components can hold and manage their state and have a separate render method for returning JSX on the screen. They are also called stateful components.


**What is the dataflow of React?**


It is also known as one-way data flow, which means the data has one, and only one way to be transferred to other parts of the application. In essence, this means child components are not able to update the data that is coming from the parent component. In React, data coming from a parent is called props.

![dataflow](https://csharpcorner-mindcrackerinc.netdna-ssl.com/article/what-and-why-reactjs/Images/image004.jpg)


**How do we make a React element a DOM element?**

ReactDOM does not render a React component or a React element in the DOM. It renders DOM elements backed by instances of their components. This is true for class components. For function components, ReactDOM renders just DOM elements. Function components don’t have instances (that can be accessed with this) so when using a function component, ReactDOM renders a DOM element generated from the function’s returned element.

* Call React.createElement() and describe its arguments.

* Use ReactDOM.render() to render an element to a page.

* Describe how we can build elements out of other React elements

* Add child elements and nested child elements.

* Pass properties to an element


![Dom](https://cdn-media-1.freecodecamp.org/images/1*mXjNHOx9bbQ5D4sSUAX2Lg.png)