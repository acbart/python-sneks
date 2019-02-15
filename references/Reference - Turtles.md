The following documents how to use the Turtle module. The [official Python
Documentation](https://docs.python.org/3.0/library/turtle.html) has more
information about these and other methods related to Turtle graphics.

Overall, you should think of the Turtle canvas as a 2-dimensional grid (an XY
plane) of pixels. The Turtle starts at (0, 0), which is in the center of the
window, and faces to the right (east). The top-right corner is positive X and
positive Y, and the bottom-left corner is the negative X and negative Y.

# Table of Contents

  * [Table of Contents](#table-of-contents_1)
  * [Movement](#movement)
    * [forward](#forward)
    * [backward](#backward)
    * [right](#right)
    * [left](#left)
  * [Jumping](#jumping)
    * [goto](#goto)
    * [setx](#setx)
    * [sety](#sety)
    * [setheading](#setheading)
  * [Special Movement](#special-movement)
    * [circle](#circle)
    * [speed](#speed)
  * [Pen](#pen)
    * [pendown](#pendown)
    * [penup](#penup)
    * [pensize](#pensize)
    * [color](#color)

# Movement

These methods allow you to move the turtle in simple ways.

## forward

**Description**: Move the turtle forward by the specified `distance`, in the direction the turtle is headed.  
**Syntax**:
```python

turtle.forward(distance)

```

**Parameters**:  
\- distance (`int` or `float`): The number of pixels to move ahead by.

**Examples**:
```python

turtle.forward(100)
turtle.forward(25)
turtle.forward(-72)

```

**Full Documentation**:[forward](https://docs.python.org/3.0/library/turtle.html#turtle.forward)

* * *

## backward

**Description**: Move the turtle backward by `distance`, opposite to the direction the turtle is headed. Do not change the turtle’s heading.  
**Syntax**:
```python

turtle.backward(distance)

```

**Parameters**:  
\- distance (`int` or `float`): The number of pixels to move back by.

**Examples**:
```python

turtle.backward(100)
turtle.backward(25)
turtle.backward(-72)

```

**Full Documentation**:[backward](https://docs.python.org/3.0/library/turtle.html#turtle.backward)

* * *

## right

**Description**: Turn turtle right by `angle` degrees (clockwise).  
**Syntax**:
```python

turtle.right(angle)

```

**Parameters**:  
\- angle (`int` or `float`): The number of degrees to turn.

**Examples**:
```python

turtle.right(90)
turtle.right(342)
turtle.right(-45)

```

**Full Documentation**:[right](https://docs.python.org/3.0/library/turtle.html#turtle.right)

* * *

## left

**Description**: Turn turtle left by `angle` degrees (counter-clockwise).  
**Syntax**:
```python

turtle.left(angle)

```

**Parameters**:  
\- angle (`int` or `float`): The number of degrees to turn.

**Examples**:
```python

turtle.left(90)
turtle.left(342)
turtle.left(-45)

```

**Full Documentation**:[left](https://docs.python.org/3.0/library/turtle.html#turtle.left)

# Jumping

These methods make the Turtle move to an absolute position instead of a
relative position.

## goto

**Description**: Move turtle to an absolute position. If the pen is down, draw line. Do not change the turtle’s orientation.  
**Syntax**:
```python

turtle.goto(x, y)

```

**Parameters**:  
\- x (`int` or `float`): The horizontal position on the screen (negative is
left of center, positive is right of center).  
\- y (`int` or `float`): The vertical position on the screen (negative is
above center, positive is below center).

**Examples**:
```python

turtle.goto(0, 0)
turtle.goto(100, 100)
turtle.goto(-27, 83)

```

**Full Documentation**:[goto](https://docs.python.org/3.0/library/turtle.html#turtle.goto)

* * *

## setx

**Description**: Move turtle to an absolute horizontal position, without affecting its vertical position. If the pen is down, draw line. Do not change the turtle’s orientation.  
**Syntax**:
```python

turtle.setx(x)

```

**Parameters**:  
\- x (`int` or `float`): The horizontal position on the screen (negative is
left of center, positive is right of center).

**Examples**:
```python

turtle.setx(0)
turtle.setx(100)
turtle.setx(-27)

```

**Full Documentation**:[setx](https://docs.python.org/3.0/library/turtle.html#turtle.setx)

* * *

## sety

**Description**: Move turtle to an absolute vertical position, without affecting its horizontal position. If the pen is down, draw line. Do not change the turtle’s orientation.  
**Syntax**:
```python

turtle.sety(y)

```

**Parameters**:  
\- y (`int` or `float`): The vertical position on the screen (negative is
above center, positive is below center).

**Examples**:
```python

turtle.sety(0)
turtle.sety(100)
turtle.sety(-27)

```

**Full Documentation**:[sety](https://docs.python.org/3.0/library/turtle.html#turtle.sety)

* * *

## setheading

**Description**: Set the orientation of the turtle to `angle`, so that it faces a certain direction.  
**Syntax**:
```python

turtle.setheading(angle)

```

**Parameters**:  
\- angle (`int` or `float`): The new angle in degrees. So 0 is east, 90 is
north, 180 is west, and 270 is south.

**Examples**:
```python

turtle.setheading(0)
turtle.setheading(90)
turtle.setheading(-127)

```

**Full Documentation**:[setheading](https://docs.python.org/3.0/library/turtle.html#turtle.setheading)

* * *

# Special Movement

These functions are more interesting ways of moving the Turtle.

## circle

**Description**: Draw a circle with given radius. The center is `radius` units left of the turtle.  
**Syntax**:
```python

turtle.circle(radius)

```

**Parameters**:  
\- radius (`int` or `float`): How wide the circle is (half of its diameter).

**Examples**:
```python

turtle.circle(1)
turtle.circle(20)
turtle.circle(500)

```

**Full Documentation**:[circle](https://docs.python.org/3.0/library/turtle.html#turtle.circle)

* * *

## speed

**Description**: Set the turtle’s speed to an integer value in the range 0-10. Speeds from 1 to 10 enforce increasingly faster animation of line drawing and turtle turning. A speed of 0 is instantenous, but a speed of 1 is very slow and a speed of 10 is very fast.  
**Syntax**:
```python

turtle.speed(speed)

```

**Parameters**:  
\- speed (`int` or `float`): A number from 0-10 indicating how fast the turtle
should move.

**Examples**:
```python

turtle.speed(0)
turtle.speed(1)
turtle.speed(6)

```

**Full Documentation**:[speed](https://docs.python.org/3.0/library/turtle.html#turtle.speed)

* * *

# Pen

These methods affect the pen that the Turtle is carrying. In general, the pen
can be on or off, and you can change its color and size.

## pendown

**Description**: Pull the pen down - in other words, the turtle WILL draw when moving.   
**Syntax**:
```python

turtle.pendown()

```

**Examples**:
```python

turtle.pendown()

```

**Full Documentation**:[pendown](https://docs.python.org/3.0/library/turtle.html#turtle.pendown)

* * *

## penup

**Description**: Pull the pen up - in other words, the turtle will NOT draw when moving.   
**Syntax**:
```python

turtle.penup()

```

**Examples**:
```python

turtle.penup()

```

**Full Documentation**:[penup](https://docs.python.org/3.0/library/turtle.html#turtle.penup)

* * *

## pensize

**Description**: Set the line thickness to `width`.  
**Syntax**:
```python

turtle.pensize(width)

```

**Parameters**:  
\- width (`int`): A positive number.

**Examples**:
```python

turtle.pensize(1)
turtle.pensize(3)
turtle.pensize(10)

```

**Full Documentation**:[pensize](https://docs.python.org/3.0/library/turtle.html#turtle.pensize)

* * *

## color

**Description**: Set the line’s color to `color`. There are a surprisingly large number of options: you can find a complete list of colors available [here](https://www.tcl.tk/man/tcl8.4/TkCmd/colors.htm).  
**Syntax**:
```python

turtle.color(color)

```

**Parameters**:  
\- color (`str`): A string with the name of the new color.

**Examples**:
```python

turtle.color('black')
turtle.color('red')
turtle.color('light goldenrod yellow')

```

**Full Documentation**:[color](https://docs.python.org/3.0/library/turtle.html#turtle.color)