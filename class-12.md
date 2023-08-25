# *Course 201, Entry 12:  Chart.js, Canvas*

Graphics and charts offer a lot of value for a page. Via Canvas and Chart.js, pages can be amplified in their delivery. 

## JavaScript Canvas

With Canvas, a developer can add 2D graphics. This is initiated by creating a `<canvas>` tag, with width and height attributes therein. These can later be changed via the following syntax:

```
const canvas = document.querySelector('#canvas');

canvas.width = 600;
canvas.height = 400;
```

Unlike image elements, the canvas element needs a closing tag. This is because within the tags is fallback content.

### getContext() method

The `getContext()` method take jsut one argument, the context type. An example of pulling the 2D context method is as follows:

```
let canvas = document.querySelector('#canvas');
let ctx = main.getContext('2d');
```

### 2D Drawing Context 

The 2D drawing context has two main options, `fillStyle` and `strokeStyle`. These are complete using the VI quadrant for an X and Y axis coordinate.

Example: 

```
(() => {
    const canvas = document.querySelector('#main');
    if (!canvas.getContext) {
        return;
    }

    // get the context
    let ctx = canvas.getContext('2d');

    // set fill and stroke styles
    ctx.fillStyle = '#F0DB4F';
    ctx.strokeStyle = 'red';

    // draw a rectangle with fill and stroke
    ctx.fillRect(50, 50, 150, 100);
    ctx.strokeRect(50, 50, 150, 100);

})();
```
Output: 

![2D Canvas Draw example](/canvasdraw.png)[^1]

The first two numbers in each parameter represent where to start, while the last two numbers represent the width and height.

## Chart.js



Chart types:



+ 
+ 
+ 

### Animated Charts



## Things I want to know more about


[^1]: Source: https://www.javascripttutorial.net/web-apis/javascript-canvas/

https://www.javascripttutorial.net/sample/webapis/canvas/