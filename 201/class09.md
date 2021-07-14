
# Lists, Tables & Forms

## Forms

There are several types of form controls that
you can use to collect information from visitors
to your site.

* ADDING TEXT:

   Text input (single-line)
    Used for a single line of text such
    as email addresses and names. 

    Password input
 Like a single line text box but it
 masks the characters entered.

   Text area (multi-line)
    For longer areas of text, such as
    messages and comments.

* Making Choices:

    Radio buttons
    For use when a user must select
    one of a number of options

    Checkboxes
    When a user can select and
    unselect one or more options.
    
     Drop-down boxes
    When a user must pick one of a
    number of options from a list.


*  Submitting Forms:

    Submit buttons, Image buttons

*  Uploadi ng Files:

    File upload
    Allows users to upload files
    (e.g. images) to a website.


![form](https://www.researchgate.net/profile/Salah-Alkhafaji/publication/318561240/figure/fig4/AS:631677474840580@1527615054215/Form-to-input-data-62-Teaching-Resource.png)


**Form Structure**

* < form>
Form controls live inside a
< form> element. This element
should always carry the action
attribute and will usually have a
method and id attribute too.

    
* action
Every < form> element requires
an action attribute. Its value
is the URL for the page on the
server that will receive the
information in the form when it
is submitted.

* method
Forms can be sent using one of
two methods: get or post.

```html
<form action="http://www.example.com/subscribe.php"
method="get">
<p>This is where the form controls will appear.
</p>
</form>

```

**Text Input**

```html 
<form action="http://www.example.com/login.php">
<p>Username:
<input type="text" name="username" size="15"
maxlength="30" />
</p>
</form>
```
* < input> : The < input> element is used
to create several different form
controls.

* type="text"
When the type attribute has a
value of text, it creates a singleline
text input.

**Password Input**

```html
<form action="http://www.example.com/login.php">
<p>Username:
<input type="text" name="username" size="15"
maxlength="30" />
</p>
<p>Password:
<input type="password" name="password" size="15"
maxlength="30" />
</p>
</form>

```

* < input>
type="password"
When the type attribute has
a value of password it creates
a text box that acts just like a
single-line text input, except
the characters are blocked out.

* name
The name attribute indicates
the name of the password input.


**Text Area**

```html
< textarea>
The < textarea> element
is used to create a mutli-line
text input

```

## Css for List, table ,forms

**Bullet Point Styles**

list-style-type : The list-style-type property
allows you to control the shape
or style of a bullet point

It can be used on rules that
apply to the < ol>, < ul>, and < li>
elements.

Unordered Lists

For an unordered list you can use
the following values:

none ,
disc ,
circle ,
square

Ordered Lists

For an ordered (numbered) list
you can use the following values:

decimal
1 2 3

decimal-leading-zero
01 02 03

lower-alpha
a b c

upper-alpha
A B C

lower-roman
i. ii. iii.


```html 

ol {
list-style-type: lower-roman;}
```

**Images for Bullets**

list-style-image

You can specify an image to act
as a bullet point using the
list-style-image property.

The value starts with the letters
url and is followed by a pair
of parentheses. Inside the
parentheses, the path to the
image is given inside double
quotes.


```html
ul {
list-style-image: url("images/star.png");}
li {
margin: 10px 0px 0px 0px;}

```

**list-style-position**

This property can take one of
two values:

* outside
    The marker sits to the left of the
    block of text. 

* inside
  The marker sits inside the box of
  text.


```html 
ul.illuminations {
list-style-position: outside;}
ul.season {
list-style-position: inside;}
```

**Table Properties**

You have already met several
properties that are commonly
used with tables.

* width to set the width of the
table

* padding to set the space
between the border of each table

* text-transform to convert the
content of the table headers to
uppercase

* text-align to align the writing
to the left of some table cells and
to the right of the others.

* background-color to change
the background color of the
alternating table rows.

* :hover to highlight a table row
when a user's mouse goes over it

## Event

Events are the browser's way of indicating when
something has happened (such as when a page has
finished loading or a button has been clicked).

Scripts often respond to these events by updating the content of the web page (via the
Document Object Model) which makes the page feel more interactive.

* UI EVENTS Occur when a user interacts with the browser's user interface (UI) rather than the web page

    * load : Web page has finished loading
    
    * unload: Web page is unloading
    
    * scroll: User has scrolled up or down the page

* KEYBOARD EVENTS Occur when a user interacts with the keyboard (see also input event)

    * keydown
    * keyup
    * keypress

* MOUSE EVENTS Occur when a user interacts with a mouse. trackpad, or touchscreen

    * click : User presses and releases a button over the same element

    * mousedown: User presses a mouse button while over an element

    * mousemove: User presses a mouse button while over an element

**HOW EVENTS TRIGGER
JAVASCRIPT CODE**

1. Select t he element
node(s) you want the
script to respond to.

2. Indicate which event on
the selected node(s) will
trigger the response.

3. State the code you want
to run when the event
occurs

how event handling can be used to provide feedback to
users filling in a registration form. It will show an error message if their
username is too short.

* SELECT ELEMENT
* SPEC!FY EVENT
* CALL CODE

![event](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/07/Ways-of-Using-JavaScript-Events-1200x720.png)

**Here is the syntax to bind an event to an element using an event listener**

element .addEventlistener('event', functionName [, Boolean]) ;

![addevent](https://cdn.tutsplus.com/active/uploads/legacy/flashtuts/074_EventListenersBasics/1.jpg)






