# Readings: Redux - Asynchronous Actions


# Review, Research, and Discussion


* How granular should your reducers be?

         It is difficult to manage states that are deeply nested, so more reducers is better than only a few. Redux gives us combineReducers to let us define more precisely what our initial state will look like.

* Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched
        Con :Dispatching an action within a reducer is an anti-pattern. Your reducer should be without side effects, simply digesting the action payload and returning a new state object. Adding listeners and dispatching actions within the reducer can lead to chained actions and other side effects.

         you can now dispatch multiple actions from one dispatch call
* Name a strategy for preventing the above

        Make a reducer for each component that will be affected by the dispatcher

# Term

* store: is basically just a plain JavaScript object that allows components to share state.
* combined reducers: helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore

# Preview

* Which 3 things had you heard about previously and now have better clarity on?

            store
* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    
         combined reducers
* What are you most excited about trying to implement or see how it works?

        combined reducers



# Preparation Materials

**async actions**

how to use the React-Redux library to let our React components interact with a Redux store, including calling useSelector to read Redux state, calling useDispatch to give us access to the dispatch function, and wrapping our app in a <Provider> component to give those hooks access to the store.

So far, all the data we've worked with has been directly inside of our React+Redux client application. However, most real applications need to work with data from a server, by making HTTP API calls to fetch and save items.

**Redux Async Data Flow​**

So how do middleware and async logic affect the overall data flow of a Redux app?

Just like with a normal action, we first need to handle a user event in the application, such as a click on a button. Then, we call dispatch(), and pass in something, whether it be a plain action object, a function, or some other value that a middleware can look for.

[Async Redux](https://redux.js.org/tutorials/fundamentals/part-6-async-logic)