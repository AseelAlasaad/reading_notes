# Reading: Context API - Behaviors

# Review, Research, and Discussion

* When you have multiple contexts, what component type should you use (class/function) and why?

    The static contextType property won't work if you need more than one, so instead you need to use a context consumer.
* How can you best test context?
  
    
    The best way to test Context is to make our tests unaware of its existence and avoiding mocks. We want to test our components in the same way that developers would use them (behavioral testing) and mimic the way they would run in our applications (integration testing).


# Term

* context: React Context is a method to pass props from parent to child component(s)

* useContext():  used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level

* static context: property is used to consume a context created with React. ... When the property is specified for a React component, you can access the current value of the context using this


# Preview


* Which 3 things had you heard about previously and now have better clarity on?

    static context

* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

    useContext

* What are you most excited about trying to implement or see how it works?
    
     useContext


# Preparation Materials

**context api**

Context provides a way to pass data through the component tree without having to pass props down manually at every level.

In a typical React application, data is passed top-down (parent to child) via props, but such usage can be cumbersome for certain types of props (e.g. locale preference, UI theme) that are required by many components within an application. Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.

**When to Use Context**

Context is designed to share data that can be considered “global” for a tree of React components

