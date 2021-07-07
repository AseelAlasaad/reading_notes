# HTML
## Images, Color, Text



 cp12 264-299

Images can be used to set the tone for a site in less time than it takes to read a description.

####  Storing Images on Your Site
If you are building a site from scratch, it is good
practice to create a folder for all of the images
the site uses.
As a website grows, keeping
images in a separate folder
helps you understand how the
site is organized

![images](https://slidetodoc.com/presentation_image_h2/61d5bf52be95a1b120eda3b5ca2378d5/image-9.jpg)

#### Adding Images

< img > 
To add an image into the page
you need to use an < img>
element. This is an empty
element (which means there is
no closing tag). It must carry the
following two attributes:

* src
This tells the browser where
it can find the image file. This
will usually be a relative URL
pointing to an image on your
own site.

* alt
This provides a text description
of the image which describes the
image if you cannot see it.

Example:

```html
<img src="images/quokka.jpg" alt="A family of
quokka" />


```

**Height & Width of Images**

You will also often see an < img>
element use two other attributes
that specify its size:

* height
This specifies the height of the
image in pixels.

* width
This specifies the width of the
image in pixels.

examples of image placement
that produce different results:

1. before a paragraph
```html
<img src="images/bird.gif" alt="Bird" width="100"
height="100" />
<p>There are around 10,000 living species of birds</p>

```

2. inside the start of a
paragraph

```html
<p><img src="images/bird.gif" alt="Bird" width="100"
height="100" />There are around 10,000 living
species of birds that inhabit different
ecosystems from the Arctic.</p>

```

3. in the middle of a
paragraph

```html
<p>There are around 10,000 living species of birds
that inhabit different ecosystems from the
Arctic to the Antarctic.<img
src="images/bird.gif" alt="Bird" width="100"
height="100" />Many species undertake long
distance annual migrations, and many more perform
shorter irregular journeys.</p>

```

*Image Resolution*

bitmap images

JPGs, GIFs, and PNGs belong to
a type of image format known
as bitmap. They are made up of
lots of miniature squares. The
resolution of an image is the
number of squares that fit within
a 1 inch x 1 inch square area.Images appearing on computer
screens are made of tiny squares
called pixels.

**Images created for the web should be saved at
a resolution of 72 ppi (pixels per inch). The higher the resolutionof the image, the larger the size of the file.**

Vector images 

Vector images differ from bitmap images and
are resolution-independent. Vector images are
commonly created in programs such as Adobe
Illustrator.

#### Figure and Figure Caption

< figure>
Images often come with
captions. HTML5 has introduced
a new < figure> element to
contain images and their caption
so that the two are associated.You can have more than one
image inside the < figure>
element.


< figcaption>
The < figcaption> element has
been added to HTML5 in order
to allow web page authors to add
a caption to an image.


## COLOR

Color can really bring your pages to life.
The color property allows you
to specify the color of text inside
an element. You can specify any
color in CSS in one of three ways:

* rgb values

   color: #ee3e80;

* hex codes

   color: rgb(100,100,90);

* color names
   
   color: DarkCyan;

You can specify your choice of
background color in the same
three ways you can specify
foreground colors: RGB values,
hex codes, and color names 

background-color: rgb(200,200,200);

background-color: DarkCyan;

background-color: #ee3e80;

#####  HSl Colors

CSS3 introduces an entirely new and intuitive
way to specify colors using hue, saturation,
and lightness values.

**Hue** is the colloquial idea of
color. In HSL colors, hue is often
represented as a color circle
where the angle represents the
color, although it may also be
shown as a slider with values
from 0 to 360.

**Saturation** is the amount of
gray in a color. 

**Lightness** is the amount of
white (lightness) or black
(darkness) in a color.

## TEXT

Choosing a Typeface
for your Website, When choosing
a typeface, it
is important to
understand that a
browser will usually
only display it if it's
installed on that
user's computer.

Serif
Serif fonts have extra details on
the end of the main strokes of
the letters.
Examples:
Georgia,
Times,
Times New Roman

Sans-Serif
Sans-serif fonts have straight
ends to letters and therefore
have a much cleaner design.
Examples:
Arial,
Verdana,
Helvetica

There are several ways to use fonts other than those listed .

The font-family property
allows you to specify the
typeface that should be used for
any text inside the element,The value of this property is the
name of the typeface you want
to use.

Example:

body {
font-family: Georgia, Times, serif;}

**font-size**: The font-size property enables
you to specify a size for the
font.

Example:

body {
font-family: Arial, Verdana, sans-serif;
font-size: 12px;}

**font-weight**: the property
allows you to create bold text.
There are two values that this
property commonly takes:

* normal
This causes text to appear at a
normal weight.

* bold
This causes text to appear bold.

If you want to create italic text,
you can use the **font-style**
property. There are three values
this property can take:

* normal
This causes text to appear in a
normal style .

* italic
This causes text to appear italic.

* oblique
This causes text to appear
oblique.

The **text-transform** property
is used to change the case of
text giving it one of the following
values:

* uppercase
This causes the text to appear
uppercase.

* lowercase
This causes the text to appear
lowercase.

* capitalize
This causes the first letter of
each word to appear capitalized.

You can control the space between lines of text,
individual letters, and words. Text can also be aligned
to the left, right, center, or justified. It can also be
indented.