## Website Performance Optimization portfolio project

### How to access website

1. The website can be accessed by navigating to the following site in your browser: [https://sambritney.github.io/frontend-nanodegree-mobile-portfolio/](https://sambritney.github.io/frontend-nanodegree-mobile-portfolio/)

### Optimizations

####Increase page speed
1. Images were resized to more closely align with their natural size and compressed with imageOptim (pizzeria.jpg & profilepic.jpg).
2. Inlined above-the-fold CSS (style.css to index.html) using grunt-critical.
3. Used Web Font Loader to reduce font loading time
4. Added async attribute to analytics.js to prevent it from being render-blocking.
5. Added media query to print.js to prevent it from being render-blocking.

####Improve scrolling performance to 60fps
1. Moved vairables out of `for loop` in main.js (updatePositions function).
2. Created new `for loop` to create static values used in another loop (updatePositions function).
3. Changed querySelectorAll to getElementsByClassName (updatePositions function).
4. Added CSS hack to render pizzas in their own layer. Note: could possibly affect performance if GPU is weak.

####Time to resize pizzas less than 5ms
1. Moved vairables out of `for loop` in main.js (changePizzaSizes function).
