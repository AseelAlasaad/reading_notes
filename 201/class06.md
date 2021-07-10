# Function

When you call a function that had parameters, you specify the values it should use in the parentheses that follow its name. The value are called arguments.

**Parameters VS Arguments**

parameters: when function is declared you can see the variables (in parentheses on the first line) inside the curly braces of the function.

Arguments: when the function is called  that has parameters ,you specify the value it should use in the parentheses that follow  its name.

* some function return a value and some function can return more than one value. 

FUNCTION DECLARATION:

A function declaration creates a function that you
can ca ll later in your code.you
must give it a name, so these are known as named
functions


FUNCTION EXPRESSION:

A function with no name is called an anonymous
function. the function expression is stored in a variable.

![function](https://image.slidesharecdn.com/javascriptppt-130607080348-phpapp01/95/java-script-ppt-10-638.jpg?cb=1403847045)

**IMMEDIATELY INVOKED FUNCTION**

these functions are not given
a name. Instead, they are executed once as the
interpreter comes across them.This way of writing a function is used in several different situations.
Often functions are used to ensure that the variable names do not conflict
with each other.

The location where you declare a variable will affect where it can be used
within your code. If you declare it within a function, it can only be used
within that function. This is known as the variable's scope.
 
* global variable:

   when create a variable outside of a function.

* local variable:

   When a variable is created inside a function.







# Document Object Model (DOM)

The Document Object Model (DOM) specifies
how browsers should create a model of an HTML
page and how JavaScript can access and update the
contents of a web page while it is in the browser window.

The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules.
It is implemented by all major browser makers, and covers two primary areas:

* MAKING A MODEL OF THE HTML PAGE: When the browser loads a web page, it
creates a model of the page in memory.The DOM specifies the way in which the
browser should structure this model using
a DOM tree.
The DOM is called an object model
because the model (the DOM tree) is
made of objects.

* ACCESSING AND CHANGING THE HTML PAGE: The DOM also defines methods and
properties to access and update each
object in this model, which in turn updates
what the user sees in the browser.
You will hear people call the DOM an
Application Programming Interface (API).

![dom](https://cf.ppt-online.org/files/slide/l/lG6hjyFR8carDYH7oVAtPW3exEOg0sSpQ1JKfm/slide-4.jpg)

all of
the element nodes are described using the same
terms as a family tree: parents, children, siblings,
ancestors, and descendants

### WORKING WITH THE DOM TREE

Accessing and updating the DOM tree involves two steps:

1. Locate the node that represents the element you want to work with.
2. Use its text content, child elements, and attributes.

STEP 1: ACCESS THE ELEMENTS

* SELECT AN INDIVIDUAL
ELEMENT NODE

Here are three common ways to
select an individual element:

   1. getElementByld ()
     Uses the value of an element's
     id attribute
     
     
```html
<hl id="header">List King<lhl>
<h2>Buy groceries<lh2>
<ul>
<li id="one" class="hot"><em>fresh<lem>
figs<lli>
<li id="two" class="hot">pine nut s<lli>
<li id="three" class="hot">honey<lli>
<li id="four">balsamic vi negar<ll i>
</ul>

JS code:
 **Select the element and store it in a variable.**

   var el = document.getElementByid('one');

 **Change the value of the class attribute.**
  el.className ='cool ' ;

 ```

   2. querySe1ector ()
   Uses a CSS selector, and returns
   the first matching element.



* SELECT MULTIPLE
ELEMENTS

  There are three common ways to
select multiple elements.

1. getElementsByClassName()
Selects all elements that have
a specific value for their cl ass
attribute.

2. getElementsByTagName()
Selects all elements that have the
specified tag name ..

3. querySelectorAll()
Uses a CSS selector to select all
matching elements.


* TRAVERSING BETWEEN
ELEMENT NODES


STEP 2: WORK WITH THOSE ELEMENTS

ACCESS/ UPDATE
TEXT NODES

The text inside any element is
stored inside a text node. To
access the text node.
1. Select the element
2. Use the firstChil d property
to get the text node
3. Use the text node's only
property (nodeVa l ue) to get
the text from the element.

WORK WITH HTML
CONTENT

One property allows access to
child elements and text content:
innerHTML
