# HTML Table

There are several types of information
that need to be displayed in a 
table.

A table represents information in a grid format.

## Table Structure

The < table> element is used
to create a table. The contents
of the table are written out row
by row.

< tr>
You indicate the start of each
row using the opening < tr> tag.
It is followed by one or more
< td> elements (one for each cell
in that row).
At the end of the row you use a
closing < /tr> tag.

< td>
Each cell of a table is
represented using a < td>
element. (The td stands for
table data.)

```html
<table>
<tr>
<td>15</td>
<td>15</td>
<td>30</td>
</tr>
<tr>
<td>45</td>
<td>60</td>
<td>45</td>
</tr>
<tr>
<td>60</td>
<td>90</td>
<td>90</td>
</tr>
</table>

```

## Table Headings

The < th> element is used just
like the < td> element its represent the
heading for either a column or
a row. (The th stands for table
heading.).


**Spanning ColumnS and Rows**

The colspan attribute in HTML specifies the number of columns a cell should span. It allows the single table cell to span the width of more than one cell or column.

The rowspan attribute can be
used on a < th> or < td> element
to indicate how many rows a cell
should span down the table.


![column](https://images.slideplayer.com/14/4212556/slides/slide_5.jpg)

There are three elements that
help distinguish between the
main content of the table:

* < thead>
The headings of the table should
sit inside the < thead> element.

* < tbody>
The body should sit inside the
< tbody> element.

* < tfoot>
The footer belongs inside the
< tfoot> element.

The border attribute was used
on both the < table> and < td>
elements to indicate the width of
the border in pixels.

Example:

```html
<table border="2" bgcolor="#efefef">
<tr>
<th width="150"></th>
<th>Withdrawn</th>
<th>Credit</th>
<th width="150" bgcolor="#cccccc">Balance</th>

```

# OBJECT

Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world

* variable become known as a Properties

    Properties te ll us about the object,

* function become known as a method

    Methods represent tasks that are associated with
the object

## Literal object

literal notation is the easiest and most papular way to create objects

![obj](https://image.slidesharecdn.com/a-reintroduction-to-javascript4633/95/a-reintroduction-to-javascript-47-728.jpg?cb=1183482021)

you can access the properties or method of an object usiing dot notation.

### CONSTRUCTOR NOTATION

You create a new object using a combination of the new keyword and Object() constructor function.

![object](https://csawesome.runestone.academy/runestone/books/published/csawesome/_images/worldConstructors.png)

to update the value of properties, use dot notation or square brackets.

to delete a property, use the delete keyword.

Once you have created an object
(using literal or constructor
notation), you can add new
properties to it.You do this using the dot
notation

Once you have created an object, the syntax for
adding or removing any properties and methods
from that object is the same.

OBJECT CONSTRUCTOR NOTATION

Example:

var hotel = new Object();

hotel.name = 'Quay';

hotel .rooms = 40 ;

OBJECT CONSTRUCTOR NOTATION

The function can be used to create multiple objects.

The this keyword is used instead of the object name.

function Hotel(name, rooms, booked) {
    
this.name = name;

this.rooms = rooms;

this.booked = booked;

**This**

The keyword this is commonly used inside functions and objects