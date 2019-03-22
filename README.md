# Smooth scroll by tag id

Demo: [https://agvolkov5.github.io/smooth-scroll-by-id/](https://agvolkov5.github.io/smooth-scroll-by-id/)

This is a simple example of crossbrowsing smooth scroll. Scroll speed is constant for various scroll distance, however it can be simply changed by replacing just one line in `script.js`:
```js
animate({
    duration: 100,
    timing: easeInOutQuad,
    draw: function(progress) {
        window.scrollTo(0, scrollYStart + progress * scrollOffset);
    }
});
```

So, there makes scroll time is constant, and scroll speed will be depended from scroll distance (from current scroll position to the element).
