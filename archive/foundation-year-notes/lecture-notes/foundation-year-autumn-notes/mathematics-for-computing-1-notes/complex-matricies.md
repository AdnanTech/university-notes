# Complex Matricies

## Inverse

### Inversing a 2x2 matrix



### Inversing a 3x3 matrix

The easiest way to this is through MATLAB. Where `x(row1_number,;) = -x(row2_number,;) + x(row1_number,;)`

A lot of rubix style is the way to solve these type of equations.

To inverse a matrix, it's like solving a rubix cube.

![](../../../../../.gitbook/assets/image%20%2892%29.png)

* Write down the matrix, with an identity matrix next to it in one big matrix

![](../../../../../.gitbook/assets/image%20%2891%29.png)

* Convert the half matrix on the left to the identity matrix, there is a general order for making the left half zeroes for this:
  * Bottom Left
  * Middle Left
  * Bottom Middle
  * Top Right
  * Middle Right
  * Middle Top
* You can also divide rows at will, they do not need to be whole numbers, as we use the determinant later to normalise.

![](../../../../../.gitbook/assets/image%20%2890%29.png)

* If there are not integers, you times the right hand side matrix by the lowest common factor \(lowest decimal that is not zero\)
* The reciprocal of this number is also called the determinant
* You can prove this is the inverse if you times the inverse by the originak matrix, and you should get the identity matrix

