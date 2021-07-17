# Image

## Size Of  Image Using CSS

 You can control the size of an
image using the width and
height properties in CSS. Specifying image sizes helps
pages to load more smoothly
because the HTML and CSS
 code will often load before the
 images.

```html
    <img src="images/magnolia-small.jpg"
    class="small" alt="Magnolia" />

    img.large {
    width: 500px;
    height: 500px;}

 ```

    use the CSS width and height
    properties to control the image
    dimensions.

### Aligning Images Using CSS

 using the float property to align
 images. There are two ways that
this is commonly achieved:

    * Float Left

    * Float Right

```html
    <img src="images/magnolia-medium.jpg"
    alt="Magnolia" class="align-right medium" />

        img.align-right {
    float: right;
    margin-left: 10px;}

```
**display**

By default, images are inline
elements. This means that they
flow within the surrounding text.
In order to center an image, it
should be turned into a blocklevel
element using the display
property with a value of block.

there are
two common ways in which you
can horizontally center an image:

* text-align
property with a value of center

* you can
use the use the margin property

#### Background Images

 The background-image  property allows you to place
 an image behind any HTML
element.The path to the image follows
the letters url, and it is put
inside parentheses and quotes.

```html

body {
background-image: url("images/pattern.gif");}

```
**Background images are often
the last thing on the page to
load.**

**Repeating Images**

The background-repeat
property can have four values:

* repeat: 
The background image is
repeated both horizontally and
vertically

* repeat-x:
The image is repeated
horizontally only

* repeat-y: 
The image is repeated vertically
only.

* no-repeat:
The image is only shown once.

**background-attachment**

property specifies whether a
background image should stay in
one position or move as the user
scrolls up and down the page. It
can have one of two values:

* fixed: 
The background image stays in
the same position on the page.

* scroll:
The background image moves
up and down as the user scrolls
up and down the page.

```html
body {
background-image: url("images/tulip.gif");
background-repeat: no-repeat;
background-attachment: fixed;}

```

**Background Position**

background-position : to specify where in the
browser window the background
image should be placed.This property usually has a pair
of values. The first represents
the horizontal position and the
second represents the vertical.

**Example**

* left top
* left center

```html
background-position: center top;
```

**If you only specify one value,
the second value will default to
center.**

**Practical Information**


**How to Identify Keywords and Phrases**

Determining which keywords to use on your site can be one of the
hardest tasks when you start to think about SEO(Search Engine
Optimization). Here are six steps that
will help you identify the right keywords and phrases for your site.

1. Brainstorm : List down the words that
someone might type into
Google to find your site. Be sure
to include the various topics,
products or services your site is
about.

2. Organize : Group the keywords into
separate lists for the different
sections or categories of your
website.

3. Research : There are several tools that let
you enter your keywords and
then they will suggest additional
keywords you might like to
consider, such as:
adwords.google.co.uk/
select/KeywordToolExternal

4. Compare

5. Refine

6. Map


As soon as people start coming to your site, you can start analyzing
how they found it, what they were looking at and at what point they are leaving. One of the best tools for doing this is a free service offered by Google called Google Analytics.

Search engine optimization helps visitors find your
sites when using search engines.

Analytics tools such as Google Analytics allow you to
see how many people visit your site, how they find it,
and what they do when they get there.
