# Passing Functions as Props


![fun](https://i.stack.imgur.com/COWdW.png)

There are several ways to make sure functions have access to component attributes like this.props and this.state.
You can use props to pass data from parent to child component => (this.props.action_name) actionName is the name of the props that can be accessed by the child component.

```html
<MyChildComponent
    name={this.name}
/>
```
in the video increment function add "one" for count when user clik on add button called "Add" if the name is match.

**Map**
The map() method in JavaScript creates an array by calling a specific function on each element present in the parent array.

Example:

```html
const numbers = [1, 2, 3, 4, 5];
const doubled = numbers.map((number) => number * 2);
console.log(doubled);


we use the map() function to take an array of numbers and double their values. We assign the new array returned by map() to the variable doubled
```

**You can build collections of elements and include them in JSX using curly braces {}**

example:

Below, we loop through the numbers array using the JavaScript map() function. We return a <li> element for each item.

```html
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li>{number}</li>
);

```

Usually you would render lists inside a component.


**Keys**

Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity.like this example:

```html
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li key={number.toString()}>
    {number}
  </li>
);
```
The best way to pick a key is to use a string that uniquely identifies a list item among its siblings. Most often you would use IDs from your data as keys

```html
const todoItems = todos.map((todo) =>
  <li key={todo.id}>
    {todo.text}
  </li>
);
```
hen you don’t have stable IDs for rendered items, you may use the item index as a key

```html
const todoItems = todos.map((todo, index) =>
  // Only do this if items have no stable IDs
  <li key={index}>
    {todo.text}
  </li>
);
```

**React** : React is a declarative, efficient, and flexible JavaScript library for building user interfaces. It lets you compose complex UIs from small and isolated pieces of code called “components”.
 A component takes in parameters, called props (short for “properties”), and returns a hierarchy of views to display via the render method.
 The render method returns a description of what you want to see on the screen.