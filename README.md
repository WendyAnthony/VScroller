jQuery VScroller
===================
VScroller is a jQuery plugin that makes your long content scrollable with a custom vertical scrollbar, featuring smooth scroll, scrolling momentum, easing, mouse wheel and touch support.

How to use it:
-------------
Load the jQuery VScroller plugin and other required resources in the document.
``` html
<script src="jquery.min.js"></script>
<script src="jquery.event.drag.min.js"></script>
<script src="jquery.vscroller.js"></script>
<script src="jquery.mousewheel.min.js"></script>
<link href="jquery.vscroller.css" rel="stylesheet">
```

Add OPTIONAL custom easing functions support.
``` html
<script src="jquery.easing.min.js"></script>
```

Wrap your content into a scrollable container.
``` html
<div class="vscroller">
  <div class="vscroller-content">
    Content goes here
  </div>
</div>
```

Enable the plugin.
``` javascript
$('.vscroller').vscroller();
```

Default plugin options.
``` javascript

$('.vscroller').vscroller({

// enable jQuery mousewheel support
mousewheel: true,

// extra easing function
easing: 'linear',

// mousewheel and keyboard arrows offset pixel count
scrollRate: 15,

// animation duration
animationDuration: 400

});
```
