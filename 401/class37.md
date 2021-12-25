# Readings: Redux - Combined Reducers


# Review, Research, and Discussion

* Why choose Redux instead of the Context API for global state?
        Context API is easy to is use as it has a short learning curve. It requires less code, and because there's no need of extra libraries, bundle sizes are reduced. Redux on the other hand requires adding more libraries to the application bundle. The syntax is complex and extensive creating unnecessary work and complexity.
* What is the purpose of a reducer?
        a reducer is a pure function that takes an action and the previous state of the application and returns the new state.
* What does an action contain?
        An action is an object that contains two keys and their values. The state update that happens in the reducer is always dependent on the value of action
* Why do we need to copy the state in a reducer?

     If the new state is different, the reducer must create new object, and making a copy is a way to describe the unchanged part.

# Term
* immutable state: an immutable object (unchangeable object) is an object whose state cannot be modified after it is created. This is in contrast to a mutable object (changeable object), which can be modified after it is created
* time travel in redux: Time travel is the ability to move back and forth among the previous states of an application and view the results in real time. With Redux, given a specific state and a specific action, the next state of the application is always exactly the same.
* action creator: An action creator is a function that literally creates an action object. In Redux, action creators simply return an action object and pass the argument value if necessary.
* reducer:  reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change. ... Redux relies heavily on reducer functions that take the previous state and an action in order to execute the next state.
* dispatch: dispatch is a function of the Redux store. You call store. dispatch to dispatch an action. This is the only way to trigger a state change. With React Redux, your components never access the store directly - connect does it for you.

# Preview

* Which 3 things had you heard about previously and now have better clarity on?

        reducer
* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

        dispatch
* What are you most excited about trying to implement or see how it works?

        dispatch

# Preparation Materials

**Redux Docs: Using Combined Reducers**

The most common state shape for a Redux app is a plain Javascript object containing "slices" of domain-specific data at each top-level key. Similarly, the most common approach to writing reducer logic for that state shape is to have "slice reducer" functions, each with the same (state, action) signature, and each responsible for managing all updates to that specific slice of state. Multiple slice reducers can respond to the same action, independently update their own slice as needed, and the updated slices are combined into the new state object.

Because this pattern is so common, Redux provides the combineReducers utility to implement that behavior. It is an example of a higher-order reducer, which takes an object full of slice reducer functions, and returns a new reducer function.

[Combined Reducers](https://redux.js.org/usage/structuring-reducers/using-combinereducers/)

```html

rootReducer = combineReducers({potato: potatoReducer, tomato: tomatoReducer})
// This would produce the following state object
{
  potato: {
    // ... potatoes, and other state managed by the potatoReducer ...
  },
  tomato: {
    // ... tomatoes, and other state managed by the tomatoReducer, maybe some nice sauce? ...
  }
}
```

The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

The resulting reducer calls every child reducer, and gathers their results into a single state object. The state produced by combineReducers() namespaces the states of each reducer under their keys as passed to combineReducers()

[combinereducers](https://redux.js.org/api/combinereducers/)