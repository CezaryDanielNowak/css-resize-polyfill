CSS Resize Polyfill
========
Resize handler for textarea or any given element.
Supports Internet Explorer, Edge, Firefox, Chrome, Safari etc.

![Browser support](/assets-demo/browser-support.png)

[link to CanIUse](http://caniuse.com/#search=resize)


Preview
---
![Edge Preview](/assets-demo/before-after.png)


How to use it
---
- copy `lib/*` or `npm install --save resize-polyfill`
- [apply Reverse engineering to demo.html :-)](/demo.html)

React integration
---
It's trivial to integrate with react:
```
import resizePolyfill from 'resize-polyfill';

class MyComponent {
  render (
    <textarea ref={(el) => {
      if (el) {
        resizePolyfill(el);
      }
    }}>
    
    </textarea>
  )
}
```

Why CSS Resize Polyfill is the best
---
- There are no many alternatives. I found just [Resizable as a part of jQuery UI](https://jqueryui.com/resizable/).
- It's really small (9.15KB uncompressed)
