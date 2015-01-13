
#HTML5 Canvas Load Complex Stage with KineticJS

To load a complex stage that originally contained images and event bindings using KineticJS,
we need to create a stage node using `Kinetic.Node.create()`, and then set the
images and event handlers with the help of selectors using the `get()` method.
Images and event handlers must be manually set because they aren't serializable.

<a class="jsbin-embed" href="http://jsbin.com/kujir/1/embed?js,output">KineticJS Load Complex Stage Demo</a><script src="http://static.jsbin.com/js/embed.js"></script>
