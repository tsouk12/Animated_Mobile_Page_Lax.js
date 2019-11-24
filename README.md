# Animated_Mobile_Page_Lax.js
Simple animated mobile page with lax.js animation for scrolling, which gives a modern design page. (Practise, First try)

Source and Information about the Lax.js what i used: https://github.com/alexfoxy/laxxx

##### Main script part for this:
```javascript
    <script src="https://cdn.jsdelivr.net/npm/lax.js"></script>
    <script>
      window.onload = function() {
        lax.setup(); // init
        const updateLax = () => {
          lax.update(window.scrollY);
          window.requestAnimationFrame(updateLax);
        };
        window.requestAnimationFrame(updateLax);
      };
    </script>
```
