# Class 12

## Canvas

The `<canvas>` element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown. `<canvas>` element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS.

## Grid

Grids are a very important part of canvas. Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at coordinate (0,0). All elements are placed relative to this origin.

To draw a rectangle, you can use `fillRect(x, y, width, height)` to draw a filled rectangle, `strokeRect(x, y, width, height)` to draw a rectangular outline, `clearRect(x, y, width, height)` to claer the specified rectangular area, making it fully transparent.

To draw paths, you can use `beginPath()` to create a new path. Once created, future drawing commands are directed into the path and used to build the path up. Those path methods are used to set different paths for objects. `closePath()` is used to add a straight line to the path, going to the start of the current sub-path. `stroke()` is used to draw the shape by stroking its outline. `fill()` Draws a solid shape by filling the path's content area.

For drawing straight lines, use the `lineTo(x,y)` method. One very useful function, which doesn't actually draw anything but becomes part of the path list described above, is the `moveTo()` function. You can probably best think of this as lifting a pen or pencil from one spot on a piece of paper and placing it on the next.

To draw arcs, you can use `arc(x, y, radius, startAngle, endAngle, anticlockwise)` to draw an arc which is centered at (x, y) position with radius r starting at startAngle and ending at endAngle going in the given direction indicated by anticlockwise (defaulting to clockwise) and `arcTo(x1, y1, x2, y2, radius)` to draw an arc with the given control points and radius, connected to the previous point by a straight line.

To apply colors to a shape, there are two important properties we can use `fillStyle` and `strokeStyle`. There are several properties which allow us to style lines. `lineWidth = value` sets the width of lines drawn in the future. `lineCap = type` sets the appearance of the ends of lines. `lineJoin = type` sets the appearance of the "corners" where lines meet. `miterLimit = value` establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes. `getLineDash()` returns the current line dash pattern array containing an even number of non-negative numbers. `setLineDash(segments)` sets the current line dash pattern. `lineDashOffset = value` specifies where to start a dash array on a line.

## Charts

Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. Chart.js is a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy. Chart.js gives you the ability to draw a line chart, a pie chart, and also a bar chart.

Example:

The example below shows a block of code that crates a chart using Chart.js.

```javascript
<canvas id="myChart" width="400" height="400"></canvas>
<script>
var ctx = document.getElementById('myChart').getContext('2d');
var myChart = new Chart(ctx, {
    type: 'bar',
    data: {
        labels: ['Red', 'Blue', 'Yellow', 'Green', 'Purple', 'Orange'],
        datasets: [{
            label: '# of Votes',
            data: [12, 19, 3, 5, 2, 3],
            backgroundColor: [
                'rgba(255, 99, 132, 0.2)',
                'rgba(54, 162, 235, 0.2)',
                'rgba(255, 206, 86, 0.2)',
                'rgba(75, 192, 192, 0.2)',
                'rgba(153, 102, 255, 0.2)',
                'rgba(255, 159, 64, 0.2)'
            ],
            borderColor: [
                'rgba(255, 99, 132, 1)',
                'rgba(54, 162, 235, 1)',
                'rgba(255, 206, 86, 1)',
                'rgba(75, 192, 192, 1)',
                'rgba(153, 102, 255, 1)',
                'rgba(255, 159, 64, 1)'
            ],
            borderWidth: 1
        }]
    },
    options: {
        scales: {
            yAxes: [{
                ticks: {
                    beginAtZero: true
                }
            }]
        }
    }
});
</script>

```

[Back to Home](README.md)
