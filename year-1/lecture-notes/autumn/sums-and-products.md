---
description: Lecture 05/10/2021
---

# Sums and Products

## Summary

* Introduction to summation \($$\sum$$ , "Sigma"\) notation
* Introduction to product \($$\prod$$ , "Pi"\) notation
* Notation for indicies

## Notation 

* Infix notation \( $$x + y$$ \)
* Postfix notation \( $$x~~y +$$ \)
* Prefix notation \( $$+~x~~y$$ \)
* Prefix and postfix notation are _sometimes_ used in computer science

### Summations

When working on a calculation that requires summing multiple operands, it can be useful to use the following notation

$$
\sum^{n}_{j=1}x_j=x_1 + x_2 + x_3 + \dots + x_n
$$

In this example, $$n$$ is the upper limit, $$1$$ is the lower limit, and $$j$$ is the summation index, similar to a loop variable in a for loop. $$x_j$$ refers to the expression that will be added to the result of the summation. 

In programming, it's similar to a for loop.

```text
sum <- 0 
for j <- 1 to n do 
    sum <- sum + x[j]
return sum 
```

If the sum is empty, such as in the following example, it will always evaluate to zero. 



$$
\sum^0_{k=1}k^2=0
$$

### Product 

The product notation is very similar to the summation notation outlined in the previous section. However, instead of summing values together, it multiplies them together. For example,

$$
\prod^n_{j=1}a_j=a_1 \cdot a_2 \cdot a_3 \cdot (\dots) \cdot a_n
$$

When expressed in code, this also looks very similar to the summation example, with the key difference of using multiplication instead of summation. 

```text
product <- 0
for j <- 1 to n do 
    product <- product * a[j]
return product 
```

Similarly to summation notation, if the product is empty, the expression will evaluate to 1. For example:

$$
\prod^{1}_{x=5}x_i=1
$$



