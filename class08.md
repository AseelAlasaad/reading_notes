# Layout

![layout](https://miro.medium.com/max/1024/1*XCZZZmhQN4rHLw2dW14BZQ.png)

Building Blocks:

This box will either be a block-level
box or an inline box.

    * Block-level elements : start on a new line

    Examples include:
    <h1> <p> <ul> <li>

    * Inline elements: flow in between
    surrounding text

    Examples include:
    <img> <b> <i>

**If one block-level element sits inside another
block-level element then the outer box is
known as the containing or parent element.**

CSS has the following positioning schemes that allow you to control
the layout of a page: normal flow, relative positioning, and absolute
positioning. You specify the positioning scheme using the position
property in CSS.

* In normal flow:  each block-level
element sits on top of the next
one. Since this is the default
way.

    position: static;


* Relative positioning : moves an
element in relation to where it
would have been in normal flow.

    position:relative

* When the position property
is given a value of absolute,
the box is taken out of normal
flow and no longer affects the
position of other elements on
the page

    position: absolute;

* Fixed positioning is a type
of absolute positioning that
requires the position property
to have a value of fixed.

    position:fixed

 The float property allows you
to take an element in normal
flow and place it as far to the
left or right of the containing
element as possible.The float property moves content to the left or right
of the page

## Screen Sizes

Different visitors to your site will have different sized screens that show
different amounts of information, so your design needs to be able to
work on a range of different sized screens.

The size of a user's screen
affects how big they can open
their windows and how much
of the page they will see.

* Screen Resolution

    Resolution refers to the number of Pixel per inch.

* Page Sizes

    web
designers often try to create pages of around 960-1000 pixels wide.

* Fixed Width Layouts:
    Fixed width layout
    designs do not
    change size as the
    user increases
    or decreases
    the size of their
    browser window.

    To create a fixed width layout,
    the width of the main boxes on
    a page will usually be specified
    in pixels (and sometimes their
    height, too).

    The fixed width layout will stay
    the same width no matter what
    ize the browser window is,

## Layout Grids

Grids set consistent proportions
and spaces between items which
helps to create a professional
looking design.


# CSS Frameworks

CSS frameworks aim to make your life easier by providing the code for
common tasks, such as creating layout grids, styling forms.
One of the most popular uses of CSS frameworks is in creating
grids to layout pages.

You can include multiple CSS files in one page.

There are two ways to add
multiple style sheets to a page:

1. Your HTML page can link
to one style sheet and that
stylesheet can use the @import
rule to import other style sheets.

2. In the HTML you can use a
separate <
link> element for
each style sheet.