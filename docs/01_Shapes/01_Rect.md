To create  a rectangle with `KineticJS`, we can instantiate a `Kinetic.Rect()` object.  For a full list of attributes and methods, check out the [Kinetic.Rect documentation](http://lavrton.github.io/KineticJS/api/Kinetic.Rect.html).

<a class="jsbin-embed" href="http://jsbin.com/mutuyu/1/embed?html,js,output">KineticJS Rect Demo</a>
<script src="http://static.jsbin.com/js/embed.js"></script>

```html
<!DOCTYPE HTML>
<html>
  <head>
    <style>
      body {
        margin: 0px;
        padding: 0px;
      }
    </style>
  </head>
  <body>
    <div id="container"></div>
    <script src="http://d3lp1msu2r81bx.cloudfront.net/kjs/js/lib/kinetic-v4.4.3.min.js"></script>
    <script defer="defer">
      var stage = new Kinetic.Stage({
        container: 'container',
        width: 300,
        height: 300
      });

      var layer = new Kinetic.Layer();

      var rect = new Kinetic.Rect({
        x: 50,
        y: 50,
        width: 100,
        height: 50,
        fill: 'green',
        stroke: 'black',
        strokeWidth: 4
      });

      // add the shape to the layer
      layer.add(rect);

      // add the layer to the stage
      stage.add(layer);
    </script>
  </body>
</html>
```