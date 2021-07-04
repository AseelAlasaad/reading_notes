# HTML And CSS

 HTML elements are used to describe the structure of the page (e.g. headings, subheadings, paragraphs).


![html css](https://blog.developers.ps/wp-content/uploads/2019/08/badges_intro_to_html_css_stage-01.png)

When creating a web page, you add tags
(known as markup) to the contents of the page.
The first one of this tags are the "Headings",Html has a six level of heading from h1 to h6.The
contents of an < h1 > element is the largest.

h1 -> for the main heading.

h2,h3... -> is used for subheading .
```html
<h1>This is a Main Heading</h1>

<h2>This is a Level 2 Heading</h2>

<h3>This is a Level 3 Heading</h3>

<h4>This is a Level 4 Heading</h4> 


you can control the size of text, color,and the fonts when used the CSS

to create a paragraph you should opening this tag < p >and closing < /p > tag.
The < b > element make the characters appear bold. for example:

< p >This is how we make a word appear < b >bold.</ b> < /p >

There are a few elements that do not have any words between an opening and closing tag such as < br/ >, you can use the line break tag < br > < br > if you wanted to add a line break inside themiddle of a paragraph.
```html
<!DOCTYPE html>
<html>
<head>
</head>
<body>
<p>
The Earth<br />gets one hundred tons heavier
  every day<br />due to falling space dust.</p>
</body>
</Html>
```

There are some text elements that are not intended to affect the
structure of your web pages, but they do add extra information to the
pages — they are known as semantic markup. some of these element:

 < strong > : The use of the < strong > element indicates that its content has strong importance,browsers will show
the contents of a < strong> element in bold.

```html
<p>
<strong>Beware:</strong> Pickpockets operate in this area.
</p>
```
< em > : browsers will show the contents of an < em> element in italic.

```html
<p>I <em>think</em> Ivy was the first.</p>```

< address > : The < address> element has quite a specific use: to contain contact details for the author of
the page. It can contain a physical address.

```html 
<address>
<p><a href="mailto:homer@example.org">
homer@example.org</a></p>
<p>742 Evergreen Terrace, Springfield.</p>
</address>
```
In Html there are different type of list:

1. Ordered lists : are lists where each item in the list is numbered.
2. Unordered lists are lists that begin with a bullet point.

## CSS

CSS allows you to create rules that specify how the content of an element should appear.CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon.

![css](https://i.pinimg.com/originals/0e/21/57/0e2157ed075e7e5400e1bf55adb08057.png)

There are three way to write the CSS:
1. Inline : include CSS rules within an element in Html page.

2. Internal : You can also include CSS rules within an HTML page by placing
them inside a < style> element, which usually sits inside the < head> element of the page.

3. External : The < link> element can be used in an HTML document to tell the
browser where to find the CSS file used to style the page.

### CSS Selectors
* Universal : all elements *{}.
* Class
* ID
* Type Selector

**CSS rules usually appear in a separate document,
although they may appear within an HTML page.**

### JavaScript
You may see JavaScript in the HTML between
opening < script> and closing < /script> tags.
The HTML < script > element is used in HTML pages
to tell the browser to load the JavaScript file (rather like
the < link > element can be used to load a CSS file).
the statements in **JS** should end with a semicolon.

Variables are used to temporarily store pieces of
information used in the script.

**How to Declare Variable in JS**

![var](https://1.bp.blogspot.com/-8UmWFTngfwY/XkVRuoPFfkI/AAAAAAAACmI/93j-FMkA9EYyoRIT1qlJ2sMUbobnWT1UgCLcBGAsYHQ/w1200-h630-p-k-no-nu/javascript_var.png)

JavaScript distinguishes between numbers (0-9),
strings (text), and Boolean values (true or false).






