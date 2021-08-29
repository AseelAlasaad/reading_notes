# Introduction to React and Components


Components let you split the UI into independent, reusable pieces, and think about each piece in isolation.

**What is a component?**

A component is a software object, intended to interact with other components, encapsulating certain functionality or a set of functionalities. It has an obviously defined interface and conforms to a recommended behavior common to all components within an architecture.

A component can have three different views − object-oriented view, conventional view, and process-related view.

**What are the charactistics of a component?**

* Reusability

Components are usually designed to be reused in different situations in different applications.

* Replaceable

 Components may be freely substituted with other similar components


* Independent

Components are designed to have minimal dependencies on other components.

**What are the advantages of using component based architecture?**

* Ease of deployment

As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.

* Reusable

they can be used to spread the development and maintenance cost across several applications or systems.


**What is Props?**

React is a component-based library which divides the UI into little reusable pieces. In some cases, those components need to communicate (send data to each other) and the way to pass data between components is by using props.

“Props” is a special keyword in React, which stands for properties and is being used for passing data from one component to another.

**Using Props in React**

Firstly, define an attribute and its value(data)

Then pass it to child component(s) by using Props

Finally, render the Props Data

```html

class ParentComponent extends Component {  
  render() {
    return (
      <h1>
        I'm the parent component.
        <ChildComponent />
      </h1>
    );
  }
}



```

Example: 

```html

class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}

```