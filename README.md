jQuery VScroller
===================
VScroller is a really small jQuery vertical scroller plugin with support for "jquery.mousewheel", "jquery.event.drag" and "jquery.easing".

How to use it:
-------------
Load jquery,event.drag and the jQuery vscroller plugin in your html page.
``` html
<script src="jquery.min.js"></script>
<script src="jquery.event.drag.js"></script>
<script src="jquery.vscroller.js"></script>
```
Load the optional jQuery mousewheel plugin for mouse wheel support.
``` html
<script src="jquery.mousewheel.min.js"></script>
```

Create a basic content block as follow.
``` html
<div class="vscroller">
    <div class="vscroller-content">
        <h3>Lorem ipsum.</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Doloribus, enim, voluptate veritatis aut sunt dicta officiis nulla cumque magnam alias qui rem doloremque! Molestias?</p>
        <h3>Lorem ipsum.</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Doloribus, enim, voluptate veritatis aut sunt dicta officiis nulla cumque magnam alias qui rem doloremque! Molestias?</p>
        <h3>Lorem ipsum.</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Doloribus, enim, voluptate veritatis aut sunt dicta officiis nulla cumque magnam alias qui rem doloremque! Molestias?</p>
        <h3>Lorem ipsum.</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Doloribus, enim, voluptate veritatis aut sunt dicta officiis nulla cumque magnam alias qui rem doloremque! Molestias?</p>
    </div>
</div>
```
Add your own CSS styles.
``` css
.vscroller {
    border: 1px solid gray;
    border-radius: 4px;
    position: relative;
    overflow: hidden;
    height: 224px;
}

.vscroller-content {
    position: relative;
    padding: 15px;
    margin-right: 5px;
}

.vscroller-scroll-body {
    position: absolute;
    right: 5px;
    top: 5px;
    background: #666;
    width: 10px;
    border-radius: 8px;
    opacity: 0.5;
    transition: opacity 0.5s;
    -webkit-transition: opacity 0.5s;
}

.vscroller-drag .vscroller-scroll-body,
.vscroller-scroll-body:hover {
    opacity: 1;
}

.vscroller-scroll {
    display: block;
    position: absolute;
    top: 0;
    left: 0;
    background: #999;
    width: 10px;
    height: 45px;
    border-radius: 8px;
    transition: background-color 0.25s;
    -webkit-transition: background-color 0.25s;
    z-index: 99;
    cursor: pointer;
}

.vscroller-scroll:focus {
    background: #ccc;
}
```
Call the plugin to create scrollbar.
``` javascript
$('.vscroller').vscroller();

```
Default settings.
``` javascript

$('.vscroller').vscroller({
    // mousewheel support
    mousewheel: false,
    // easing function
    easing: 'linear',
    // mousewheel and keyboard arrows offset pixel count
    scrollRate: 15,
    // scrolling animation duration
    animationDuration: 400
});
```
