# Create Stunning Animated Charts with Chart.js

Charts display data and are more visually appealing than tables.  
This article shows you how to create a chart with Chart.js

[https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/]

---

# Chart.js Installation

This article has installation information for Charts.js.  
Use `<canvas>` node with the script in your page to render the chart. 
Requires closing tag.

[https://www.chartjs.org/docs/latest/]

---

# Basic Usage of canvas

`<canvas>` element has two attributes: width and height.  
Can be set by using DOM properties.  
Width and height specifications are optional, default will be **300 pixels wide, 150 pixels high**

Canvas Element Example:

```
<canvas id="tutorial" width="150" height="150"></canvas>
```

Distortion may occur during rendering if CSS sizing doesn't match ratio of the initial canvas. Fix by using width and height instead.

Canvas can be styled with CSS.
No styling rules applied = fully transparent

Fallback content  for older browsers is inserted into the `<canvas>` element.

**Rendering Context** 

Script needs access to the rendering context to draw on it.

`getContext()` - parameter is type of context.

*Not good practice/don't do it: embed a script in HTML*


<br>

[https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage]

---

# Drawing Shapes with canvas

**The grid/Coordinate Space** -one unit in the grid = 1 pixel. X and Y axis. Top left corner = 0/starting point.

Rectangles and Paths. Combine paths to create other shapes.

This article covers 2D. Lists and explains functions for:

- drawing paths
- drawing a triangle
- moving the pen
- lines
- arcs
- bezier an dquadratic curves
- rectangles with rect() method
- making combinatoins
- Path2D objects
- using SVG paths


[https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes]

---

# Applying Styles and Colors

Two main properties for applying colors to a shape:

`fillStyle = color`  - fill the shape
`strokeStyle = color`  - outline color

Transparency:  
`globalAlpha` property for many shapes of same transparency  
RGBA color values applied to strokeStyle and FillStyle for individual shapes

The article has in-depth functions and info on the following:

Line Styles

- line width
- lineCap
- lineJoin
- using line dashes

Gradients

Patterns

Shadows

Canvas Fill Rules

<br>
[https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors]

---

# Drawing Text

Two methods to render text:

`fillText(text, x, y [,maxWidth])`  
`strokeText(text, x, y [, maxWidth])`

Styling text properties listed in article.

`measureText()` method - used to get width of text

<br>

[https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text]
