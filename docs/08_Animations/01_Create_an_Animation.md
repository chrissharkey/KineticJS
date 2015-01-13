
#HTML5 Canvas KineticJS Animation Tutorial

To create custom animations with KineticJS, we can use the `Kinetic.Animation`
constructor which takes two arguments, the required update function and
an optional layer, or array of layers, that will be updated with each animation frame.
The animation function is passed a `frame` object which contains a `time` property which is the number
of milliseconds that the animation has been running, a `timeDiff` property which
is the number of milliseconds that have passed since the last frame,
and a `frameRate` property which is the current frame rate in frames per second.

The update function should never redraw the stage or a layer because the animation
engine will intelligently handle that for us.
The update function should only contain logic that updates Node properties,
such as `position`, `rotation`, `scale`, `width`, `height`, `radius`, `colors`, etc.
Once the animation has been created, we can start it at anytime with the `start()` method.

For a full list of attributes and methods, check out the [Kinetic.Animation documentation](http://lavrton.github.io/KineticJS/api/Kinetic.Animation.html).

##HTML5 Canvas KineticJS Animation Template

```
<script>
  var anim = new Kinetic.Animation(function(frame) {
    var time = frame.time,
        timeDiff = frame.timeDiff,
        frameRate = frame.frameRate;

    // update stuff
  }, layer);

  anim.start();
</script>
```
