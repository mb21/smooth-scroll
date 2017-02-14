smooth-scroll
=============

smooth scrolling anchors page without framework dependency.

This is a fork of https://github.com/uniphil/smooth-scroll which is in turn a fork of https://github.com/Yappli/smooth-scroll with the following features:

 * eased (not linear) scroll
 * a function, `smoothScroll.registerTargets("querySelectorExpr")`, is exported to the global namespace. You must manually assign elements as targets for smooth scrolling.
 * scroll to a specific element: `smoothScroll.scrollTo( document.getElementById("foo") )`
 * scroll by 400px: `smoothScroll.scrollBy(400)`

Example:

```html
<a href="#menu"><!-- some custom JS shows/hides the menu -->
</a>
<ul id="menu">
  <a href="#videos">videos</a><!-- we want to smooth-scroll to these -->
  <a href="#photos">photos</a>
</ul>
<div id="videos">
  ...
</div>
<div id="photos">
  ...
</div>
```

```javascript
smoothScroll.registerTargets("#videos, #photos");
```

ta-daa

[**demo**](http://uniphil.github.io/smooth-scroll/)
