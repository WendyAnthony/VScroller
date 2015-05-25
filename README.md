jQuery VScroller
===================
VScroller is a jQuery plugin that makes your long content scrollable with a custom vertical scrollbar, featuring smooth scroll, scrolling momentum, easing, mouse wheel and touch support.

How to use it:
-------------
1. Load the jQuery VScroller plugin and other required resources in the document.
``` html
<script src="jquery.min.js"></script>
<script src="jquery.event.drag.min.js"></script>
<script src="jquery.vscroller.js"></script>
<link href="jquery.vscroller.css" rel="stylesheet">
```
2. Add OPTIONAL mouse wheel support.
``` html
<script src="jquery.mousewheel.min.js"></script>
```

3. Wrap your content into a scrollable container.
``` html
<div class="vscroller">
  <div class="vscroller-content">
    Content goes here
  </div>
</div>
```

4. Enable the plugin.
``` javascript
$('.vscroller').vscroller();
```

5. Default plugin options.
``` javascript

$('.vscroller').vscroller({

// enable jQuery mousewheel support
mousewheel: false,

// extra easing function
easing: 'linear',

// mousewheel and keyboard arrows offset pixel count
scrollRate: 15,

// animation duration
animationDuration: 400

});
```
