# Review, Research, and Discussion

* Why is the Context API useful?

  allows you to share information to any component, by storing it in a central place and allowing access to any component that requests it 
* Can a component outside of a provider get its context?


To access a React context outside of the render function, we can use the useContext hook. We create the UserContext by calling the React. createContext method with a default context value. Then in the Users component, we call the useContext hook with UserContext to accxess the current value of UserContext .
* What are some common use cases for using the Context API?
Describe “Context Hell”
