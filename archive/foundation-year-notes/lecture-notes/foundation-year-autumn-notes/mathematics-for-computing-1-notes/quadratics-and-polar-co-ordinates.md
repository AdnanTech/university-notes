# Quadratics and Polar Co-ordinates

## Lines and Curves

### Pre reading

Quadratics are just polynomials with (a power) order of 2. so anything x^2 is a quadratic polynomial

### General Form

$$
ax^2 + bx + c = 0
$$

a, b and c are the coefficients. If a is zero, the equation no longer becomes quadratic, honing in on the point that there has to be a power of 2 in the equation. b and c can be zero though.

### General Rule

A general rule for polynomials:

* If the highest power in the equation (order) is N, then the graph has N-1 “turns”
* So a quadratic has exactly 1 turn with no exceptions
* And a linear equation has no turns at all, for example

![](<../../../../../.gitbook/assets/image (12).png>)

## Curves (quadratics)

### Quadratic

A quadratic equation is a polynomial equation with the power of two. Invented by Rene Descartes, the man famous for saying "I think, therefore I am".

### Quadratics vs Linear

The key difference between a linear equation and a quadratic equation, is that in quadratic equations, each co-domain (x) value maps to 2 domains (y). Where in linear it was a 1 to 1 relationship. There is a caveat to this rule for quadratic, and that is where the has a turning point, meaning the tangent to the curve, also known as the gradient, is zero, at this point the co domain will map to only one domain value. Quadratic equations are also harder to inverse than linear equations.

### Solving Quadratics

&#x20;There are 4 main methods:

1. Factorisation
   1. (x + a)(a + b) where x = -a or x = -b
2. Completing the square
   1. (x+a)^2 + d where x = +/- sqrt(d) - a
3. Quadratic Formula
   1. See quadratic formula
4. Trial and Improvement
   1. Keep testing values till you get y = 0

### The discriminant

Some quadratic equations cannot be solved with real numbers, as they require complex numbers (imaginary number i), we can quickly check if the quadratic can be solved using the following equation, being the discriminant:

$$
b^2-4ac
$$

If the equation is > 0, we have 2 real roots (solutions) for the quadratic, so it passes the x axis at 2 seperate points,&#x20;

if it = 0, it has 2 roots that are the same, since it was one turning point

&#x20;if it is < 0, it has no **real** roots

### Imaginary Unit (i)

Since b^2 - 4ac can < 0, it gave birth the to the [imaginary number](https://en.wikipedia.org/wiki/Imaginary\_unit#Matrices)

### Excel

We can sketch out quadratic graphs in excel.

## [Polar Co-Ordinates](https://www.mathsisfun.com/polar-cartesian-coordinates.html)

Polar co-ordinates are diffrent function to a graph, for example, cartesian follows (point a, point b), where you go across a and up b to find a point on the line, that is the function. Whereas polar co-ordinates, map to (r, theta) for a point

* Where r is a real number (when squared at least), that is the radial distance from the distance
* Theta is the **anti-clockwise** angle from the x axis
* the polar origin is also considered (0, 0), as in cartesian equations
* A polar equation can directly correlate to a cartesian equation

It allows us to split a line into triangles, and hence integration, as it essentially is just a bunch of triangles

**To covert line equations (y = mx + c) into polar co-ordinates**

1. Take a point from the line which represents a right angle
2. r is the hypotenuse (sqrt(b^2 + c^2))
3. theta is tan^-1(b/c) - note the inverse tan

**To convert polar co-ordiantes (r, theta) back to a line equation**

1. The x value is (r \* cos(theta))
2. The y value is (r \* sin(theta))
3. This gives you an (x, y) value
4. Polar co-ordiantes are always from the origin, so you can use the point and (0, 0) to find the equation

### Solving polar co-ordinates

* Given equation
* Find perpendicular equation
* Make them equal to each other
* Solve for x
* Then sub x to find y
* using that, you can find r
* Using that, you can find theta

x = 3, or any vertical line, has a gradient of positive or negative infinity, this doesnt follow the rule of y = mx + c. It is NOT a function, this line creates problem in graphics chips, as it means that graphics cannot process straight lines, unless you use polar co-ordinates. x = 3 can be represented in polar co-ordinates as (3, 0) where 3 is the length towards the line, and 0 is theta

Your **retina** has high res in the center, and low res around the outside. This is where polar co-ordinates are a lot better than y= mx+c. Used in computer vision and graphics. Polar co-ordinates is the minimum distance to a line from the origin

