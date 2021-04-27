## Mouse Movement in Processing

The default sketch on openprocessing.org has the variables `mouseX` and `mouseY` that store the current x- and y-coordinates of the mouse.

![](../Images/Default_Sketch.png)

If we are trying to find the coordinates of a specific pixel, we can print these mouse coordinates to the console to help us find it.

```js
function setup() {
	createCanvas(windowWidth, windowHeight);
}

function draw() {
	print(mouseX, mouseY);
}
```

The `draw()` function will repeatedly print the coordinates to the console. Every time the mouse moves, the coordinates will get updated.

There are also built-in variables for the most recent mouse coordinates: `pmouseX` and `pmouseX` (the "p" stands for previous).

We can use this to track the movement of the mouse

```js
function setup() {
	createCanvas(windowWidth, windowHeight);
}

function draw() {
	line(pmouseX, pmouseY, mouseX, mouseY);
}
```

This program will continuously draw a line every time the mouse moves, leaving a trail of the places the cursor has been to.

![](../Images/Mouse_Trail.png)
