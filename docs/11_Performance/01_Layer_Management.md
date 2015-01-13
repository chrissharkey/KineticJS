
#HTML5 Canvas Layer Management with KineticJS

When creating KineticJS applications, the most important thing to consider,
in regards to performance, is layer management.  One of the things that makes
KineticJS stand out from other canvas libraries is that it enables us to create
individual layers, each with their own canvas elements.  This means that we can
animate, transition, or update some stage elements, while not redrawing others.
If we inspect the DOM of a KineticJS stage, we'll see that there is actually one
canvas element per layer.

This tutorial has two layers, one layer that's animated, and another static layer
that contains text.  Since there's no reason to continually redraw the text, it's placed in its own layer.

<a class="jsbin-embed" href="http://jsbin.com/weqaki/1/embed?js,output">KineticJS Layer Management Demo</a><script src="http://static.jsbin.com/js/embed.js"></script>
