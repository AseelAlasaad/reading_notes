# 5 Steps to THINK in React

![mock](https://image.slidesharecdn.com/thinkinginreact-160112103822/95/thinking-in-react-12-638.jpg?cb=1452595119)

**Step 1: Break The UI Into A Component Hierarchy**

For this step, you’ll want to have a whiteboard or a pen and paper handy. If one is not already provided, you’ll need a mockup of the app. You’ll then want to draw boxes around each of the components and assign each of them names. It helps to use the single responsibility principle when deciding what needs to be grouped together.

You’ll see here that we have five components in our app. We’ve italicized the data each component represents.

* FilterableProductTable (orange): contains the entirety of the example

* SearchBar (blue): receives all user input

* ProductTable (green): displays and filters the data collection based on user input

* ProductCategoryRow (turquoise): displays a heading for each category

* ProductRow (red): displays a row for each product


**Step 2: Build a Static Version in React**

To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props. props as a way of passing information from the parent component to its child component.don’t use state at all to build this static version. State is reserved only for interactivity.At the end of this step, you’ll have a library of reusable components that render your data model. React’s one-way data flow (also called one-way binding).

**Step 3: Identify The Minimal (but complete) Representation Of UI State**

To make your UI interactive, you need to be able to trigger changes to your underlying data model. React achieves this with state.To build your app correctly, you first need to think of the minimal set of mutable state that your app needs.

**Step 4: Identify Where Your State Should Live**

 First, you’ll need to determine which of your components will require state. Then, you’ll need to locate the single component above all of the components that need state. You can think of this component as the parent component where state will be passed down to its child components . 

 Follow these steps for each piece of state:

* Identify every component that relies on state.
* Find a common parent component.
* If there are no components that make sense, you can create a new component just to keep the state.

 **Step 5: Add Inverse Data Flow**


Inverse Data Flow allows parent components to access information in child components by having functions defined in the parent component but evoked in the child component.
 Our app now works by passing probs and state down to the necessary components. Now we need to allow data to flow back up from these components to the state.If you try to type in the input or check the box, nothing happens. That is by design. We have set the value prop of the input to be equal to the state passed in from component.
 Defining the function in the parent, passing the definition down as a prop, and invoking the function in the child by utilizing the prop is inverse data flow. This enables the parent to access information that is obtained in a child component.


