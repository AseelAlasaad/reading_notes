# Readings: React and Forms

## Forms

HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state

**Controlled Components**

In HTML, form elements such as
 ```html 
<input>, <textarea>, and <select>
```
typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().

We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.

Example:

```html
class NameForm extends React.Component {
  constructor(props) {
    super(props);
    this.state = {value: ''};

    this.handleChange = this.handleChange.bind(this);
    this.handleSubmit = this.handleSubmit.bind(this);
  }

  handleChange(event) {
    this.setState({value: event.target.value});
  }

  handleSubmit(event) {
    alert('A name was submitted: ' + this.state.value);
    event.preventDefault();
  }

  render() {
    return (

    ) 

      <form onSubmit={this.handleSubmit}>
        <label>
          Name:
          <input type="text" value={this.state.value} onChange={this.handleChange} />
        </label>
        <input type="submit" value="Submit" />
      </form>
    );
  }
}

```
**Form controls**

For textual form controls—like inputs and textareas—use the FormControl component. FormControl adds some additional styles for general appearance, focus state, sizing, and more.Use size on 
```html
<FormControl> and <FormLabel> 
```   
to change the size of inputs and labels respectively.


Example:

```html
<Form>
  <Form.Group className="mb-3" controlId="exampleForm.ControlInput1">
    <Form.Label>Email address</Form.Label>
    <Form.Control type="email" placeholder="name@example.com" />
  </Form.Group>
  <Form.Group className="mb-3" controlId="exampleForm.ControlTextarea1">
    <Form.Label>Example textarea</Form.Label>
    <Form.Control as="textarea" rows={3} />
  </Form.Group>
</Form>
```
**Readonly**
Add the readOnly prop on an input to prevent modification of the input's value.
Handling Multiple Inputs

When you need to handle multiple controlled input elements, you can add a name attribute to each element and let the handler function choose what to do based on the value of event.target.name.

**The Conditional (Ternary) Operator**

the syntax of a typical if statement:

if ( condition ) {
  value if true;
} else {
  value if false;
}

the ternary operator:

condition ? value if true : value if false

* The condition is what you’re actually testing. The result of your condition should be true or false or at least coerce to either boolean value.

* A ? separates our conditional from our true value. Anything between the ? and the : is what is executed if the condition evaluates to true.

* Finally a : colon. If your condition evaluates to false, any code after the colon is executed.

**Nested Ternary**

We can nest ternary operators to test multiple conditions.

Example:

let price = isStudent ? 8 : isSenior ? 6 : 10

**Multiple operations**

It is also possible to run multiple operations within a ternary. To do this, we must separate the operations with a comma. You can also, optionally, use parenthesis to help group your code:

isStudent ? (
  price = 8,
  alert('Please check for student ID')
) : (
  alert('Enjoy the movie')
);