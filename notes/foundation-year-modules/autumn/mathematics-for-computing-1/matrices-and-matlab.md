# Matrices and MATLAB

## Matrices

### Definition

A [**matrix** ](https://www.mathsisfun.com/algebra/matrix-introduction.html)is an array of numbers represented in columns and rows, that represent something collectively. A 1D matrix \(one row vector, one column vector\) could be used to represent data, such as an audio signal, a row or column in a spreadsheet, or just an array of numbers for an eqaution. An example of a 2D matrix is below.

![A 2x2 matrix](../../../../.gitbook/assets/image%20%2817%29.png)

A is a 2×2 matrix because it has two rows and two columns. These are the **dimensions** of A.

### Reading matricies

A 2D **Matrix** can **represent** a whole **spreadsheet** if we increase the dimensions. It can also represent **simulatenous equations**, or even **images**.

We can use 3D matricies to represent a colour images, where each pixel has a RGB \(red, green, blue\) value. So for an 1000x1000 image, we need a 3D matrix of size of \(1000, 1000, 3\)

In general a matrix is **m x n** matrix if it has **m rows** and **n columns**. Where m and n are the elements of the matrix. We often use square bracket notation, with subscripts, where the numbers 13 are first row, third column.

![](../../../../.gitbook/assets/image%20%2838%29.png)

A special cause of the matrix sqaure, is where m = n, not m x n

![](../../../../.gitbook/assets/image%20%2815%29.png)

### Identity matrix

Denoted as I \(capital i\), **all elements are zero apat from the top left to the bottom right, where they are 1's**

![](../../../../.gitbook/assets/image%20%2843%29.png)

## Matrix Operations

Matrix operations are used a lot in image processing. Mainly adding/subtracting, and transposing

### Adding or Subtracting Matrices

Works if only they are the same dimensions. Image processing would be superposition of images.

![](../../../../.gitbook/assets/image%20%2822%29.png)

### Transposing matricies

For matrix M, denoted as M^T. You s**wap the rows and column**. Also used in image processing to change the resolution \(for example landscape to portrait\).

![](../../../../.gitbook/assets/image%20%2839%29.png)

### Scalar multiplication

This is where you times the matrix by an some constant scalar value, aka an integer, forumla below. This is used in image processing to change the brightness.

![](../../../../.gitbook/assets/image%20%2820%29.png)

### Matrix Multiplication

Works only when the number of columns of one matrix, is equal to the number of rows of the other. Multiply each element of the rows of the first matrix by the column of the second. Used in image processing to scale up an image.

![Basic formula for a 2x2 matrix multiplacation](../../../../.gitbook/assets/image%20%2816%29.png)

![Example 1](../../../../.gitbook/assets/image%20%2833%29.png)

![Example 2](../../../../.gitbook/assets/image%20%2824%29.png)

### Matrix Division

Not clear division. Like non matrix maths, division can be abstracted to multiplacation of the reciprocal. Same applies to matricies?

### Inverse matrices

The inverse of a matrix can be seen as M^-1. Any matrix mutliplied by it's inverse matrix, will give the identity matrix. This one is more like the reciprocal matrix, but we call it the inverse matrix.

![Example 1](../../../../.gitbook/assets/image%20%2819%29.png)

![Example 2](../../../../.gitbook/assets/image%20%2835%29.png)

### Finding the Inverse

There are a few approaches, let's start with a 2x2 matix:

![](../../../../.gitbook/assets/image%20%2837%29.png)

Where _Det_ is the determinant of a matrix and is defined as a single value \(ad-bc\). _Det\(A\)_ can also be written as _\|A\|._

Let's take the original equation that is broken down into the subset of smaller matricies \(from next chapter\):

![Equation](../../../../.gitbook/assets/image%20%2834%29.png)

![Solved using Inverse method](../../../../.gitbook/assets/image%20%2830%29.png)

So from the solved equation, we can see that x is 1 and y is 2.

Inverse of a 3x3 matrix:

![inverse of a 3x3 matrix](../../../../.gitbook/assets/image%20%2832%29.png)

## Matrices applications

### Simultaneous equations

We can represent a multiplacation in matricies with fundamental algebra laws, here is an example of a sumultaneous equation being solved using matricies:

![This](../../../../.gitbook/assets/image%20%2836%29.png)

![Set of matricies](../../../../.gitbook/assets/image%20%2841%29.png)

![Can be represented like this](../../../../.gitbook/assets/image%20%2829%29.png)

### Gaussian elimation

Now we can see that the result matrix can be broken down into a subset of smaller matricies. we can use algebra laws to the matricies, as long as they are done on both sies. Like scaling, adding, subtracting and such.

The task of Gaussian elimination \(also called Gauss Jordan elimination\) is to create a matrix with 1’s on the diagonal \(top left to bottom right\) with 0’s below that diagonal.

[YouTube guide](https://www.youtube.com/watch?v=2j5Ic2V7wq4%20
)

Here is the equation above solved with the Gaussian elimination method:

![Solved using Gaussian Elimination](../../../../.gitbook/assets/image%20%2827%29.png)

As we can see, x = 1 and y = 2

### Solving using the inverse matrix

We can also solve with MATLAB using the equation: `M x M^-1 = I`

Here is the equation above solved with the inverse method:

![Solved using the inverse method](../../../../.gitbook/assets/image%20%2831%29.png)

### More examples

![Example 1](../../../../.gitbook/assets/image%20%2818%29.png)

![Example 1 continued](../../../../.gitbook/assets/image%20%2821%29.png)

### Rotating a matrix \(Geometry\)

![](../../../../.gitbook/assets/image%20%2823%29.png)

Kingsley's method for finding the Inverse:

![](../../../../.gitbook/assets/image%20%2844%29.png)

![](../../../../.gitbook/assets/image%20%2840%29.png)

![](../../../../.gitbook/assets/image%20%2845%29.png)

## MATLAB



MATLAB can be integrated with the programming language C

* Download MATLAB [here](http://www.sussex.ac.uk/its/services/software/owncomputer/matlab_student)

3 by 3 matrix grid:

x = \[1, 2, 3; 4, 5, 6; 7, 8, 9\]

imagesc\(var\) will print an colour image of the data. It's an image function

