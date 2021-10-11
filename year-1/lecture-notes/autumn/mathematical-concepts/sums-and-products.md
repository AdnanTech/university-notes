---
description: Lecture 05/10/2021
---

# Sums and Products

## Summary

* Introduction to summation ($$\sum$$ , "Sigma") notation
* Introduction to product ($$\prod$$ , "Pi") notation
* Notation for indicies

## Notation 

* Infix notation ( $$x + y$$ )
* Postfix notation ( $$x~~y +$$ ) 
* Prefix notation ( $$+~x~~y$$ ) 
* Prefix and postfix notation are _sometimes _used in computer science

### Summations

When working on a calculation that requires summing multiple operands, it can be useful to use the following notation

$$
\sum^{n}_{j=1}x_j=x_1 + x_2 + x_3 + \dots + x_n
$$

In this example, $$n$$ is the upper limit, $$1$$ is the lower limit, and $$j$$ is the summation index, similar to a loop variable in a for loop. $$x_j$$ refers to the expression that will be added to the result of the summation. 

In programming, it's similar to a for loop.

```
sum <- 0 
for j <- 1 to n do 
    sum <- sum + x[j]
return sum 
```

If the sum is empty, such as in the following example, it will always evaluate to zero. 

$$
\sum^0_{k=1}k^2=0
$$

Summations can also be nested, for example:

$$
\sum^{5}_{j=3} \sum^{2}_{k=1}j\cdot k = \sum^{2}_{k=1}3 \cdot k + \sum^{2}_{k=1}4 \cdot k+\sum^2_{k=1}5\cdot k
$$

The order of expansion in nested summations does not matter as they are associative. 

#### Usage

How do you write "the sum of the first $$n$$ odd numbers, is $$n^2$$"?

* First n odd numbers?
  * First odd number: 1
  * Second odd number: 3
  * Third odd number: 5
  * $$\dots$$ 
  * nth odd number: $$(2n - 1)$$ 

$$
\sum^{n}_{j=1} (2j-1)=n^2
$$

Indicies always range over integers, however, negative values are allowed. 

### Product 

The product notation is very similar to the summation notation outlined in the previous section. However, instead of summing values together, it multiplies them together. For example,

$$
\prod^n_{j=1}a_j=a_1 \cdot a_2 \cdot a_3 \cdot (\dots) \cdot a_n
$$

When expressed in code, this also looks very similar to the summation example, with the key difference of using multiplication instead of summation. 

```
product <- 0
for j <- 1 to n do 
    product <- product * a[j]
return product 
```

Similarly to summation notation, if the product is empty, the expression will evaluate to 1. For example:

$$
\prod^{1}_{x=5}x_i=1
$$

As opposed to summations, the order of operations matter, as multiplication has a higher precidence than summation. For example

$$
\prod^{3}_{i=1} \sum^{3}_{j=1}i\cdot j = \prod^{3}_{i=1} (i + 2 \cdot i + 3 \cdot i)
$$

#### Edge cases

* let $$a, b>0$$ 

$$
\log(a \cdot b)=\log(a)+\log(b)
$$

* More generally:



$$
\log\big(\prod^{n}_{i=i}x_i\big)=\sum^{n}_{k=0}\log(x_i)
$$

