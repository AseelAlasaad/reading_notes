# Chart.js, Canvas

![chart](https://miro.medium.com/max/1838/1*ZxZMc4n6XJxlNjA-p4WAKg.png)

Charts are far better for displaying data visually than tables

 A great way to get started with charts is with Chart.js ,
 a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page
 It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.
 Chart.js is an especially popular web design tool because it offers a unique trade-off between ease of use and advanced features, enabling you to create interactive charts.

 ## Creating a Chart
 
 * It's easy to get started with Chart.js. All that's required is the script included in your page along with a single  < canvas>  node to render the chart

add a < canvas> to where you want to draw the chart,The canvas element must have a unique id.

 ```html
 <canvas id="myChart" width="400" height="400"></canvas>

 ```

Chart.js comes with the following built-in chart types:

* Scatter
* Line
* Bar
* Radar
* Pie and Doughnut
* Polar Area




![scatter](https://www.excel-easy.com/smi/examples/scatter-plot.png)


Next, we need to write a script that will retrieve the context of the canvas, so add this to the foot of your body element,For example:

```html
<canvas id="buyers" width="600" height="400"></canvas>


<script>
    var buyers = document.getElementById('buyers').getContext('2d');
    new Chart(buyers).Line(buyerData);
</script>


```
Inside the same script tags we need to create our data, in this instance it’s an object that contains labels for the base of our chart and datasets to describe the values on the chart.for example

**Scatter Chart Syntax:**

```html

var myChart = new Chart("myChart", {
  type: "scatter",
  data: {},
  options: {}
});

```

**Canvas**
```html
At first sight a <canvas> looks like the <img> element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the <canvas> element has only two attributes, width and height. These are both optional . When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high.

```

The id attribute isn't specific to the < canvas> element but is one of the global HTML attributes which can be applied to any HTML element . It is always a good idea to supply an id because this makes it much easier to identify it in a script.

The < canvas> element can be styled just like any normal image (margin, border, background…). These rules, however, don't affect the actual drawing on the canvas.

### Drawing shapes with canvas

There are three functions that draw rectangles on the canvas:

* fillRect(x, y, width, height)

* strokeRect(x, y, width, height)

* clearRect(x, y, width, height)

Each of these three functions takes the same parameters.

```html
function draw() {
  var canvas = document.getElementById('canvas');
  if (canvas.getContext) {
    var ctx = canvas.getContext('2d');

    ctx.fillRect(25, 25, 100, 100);
    ctx.clearRect(45, 45, 60, 60);
    ctx.strokeRect(50, 50, 50, 50);
  }
}


```

**Colors**

 If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.

 * fillStyle = color

     ex: ctx.fillStyle = 'orange';

 * strokeStyle = color

**Drawing text**

The canvas rendering context provides two methods to render text:

* fillText(text, x, y [, maxWidth])

```html
function draw() {
  var ctx = document.getElementById('canvas').getContext('2d');
  ctx.font = '48px serif';
  ctx.fillText('Hello world', 10, 50);
}

```

* strokeText(text, x, y [, maxWidth])

There are some properties which let you adjust the way the text gets displayed on the canvas:

* font = value
* textAlign = value
* textBaseline = value
* direction = value

