## Shapes in Processing

In the default sketch, we have the command `ellipse(mouseX, mouseY, 30, 30)`. The last two arguments represent the size of the ellipse: the width is 30 pixels and the height is also 30 pixels. The first two arguments represent the x- and y-coordinate of the center of the ellipse. Let's look at the coordinate system. 

### Screen Coordinates

Coordinates in programming are different than coordinates in math. 

In math, 2-dimensional coordinates can be graphed on a Cartesian Plane like this:

![](../../Images/Cartesian_Plane.jpg)

In computer science, we don't use the Cartesian plane for coordinates. Instead, the coordinate system we use looks like this:

![](../../Images/Coordinate_Plane.jpg)

For example, if we are referring to a specific pixel in an image, we would use this coordinate system instead of the Cartesian plane. 

The idea is that this is similar to how we would refer to cells in a table: The row number followed by column number, with Row 0 Column 0 representing the cell in the top-left corner. This is also similar to how we read in English: left to right, top to bottom.

The coordinate (0, 0) is referred to as the **origin**. When programming, **the origin is always is at the top-left corner**. 

In math, the origin is at the center of the Cartesian plane. If we are only using the positive quadrant of the Cartesian plane, the origin is at the bottom-left corner.

### Rect(), Triangle(), and Line()

Here are a few other functions that draw shapes.

* `rect()` 
  * Draws a rectangle
  * The top-left vertex is (x, y)
  * Takes four parameters: x, y, width, height
* `triangle()`
  * Draws a triangle 
  * The three vertices are (x1, y1), (x2, y2), and (x3, y3)
  * Takes six parameters: x1, y1, x2, y2, x3, y3
* `line()` 
  * Draws a line
  * The startig point is (x1, y1) and the stopping point is (x2, y2)
  * Takes four parameters: x1, y1, x2, y2