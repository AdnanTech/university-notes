# Complex Differentiation

## Trig

When dy/dx\(sin\) is at zero, aka the turning point, cos x crosses the x axis, where y = 0.

thus if y = sinx, dy/dx = cosx.

We can prove using the base differentiation equation and trig equations

![](../../../../../.gitbook/assets/image%20%2880%29.png)

![](../../../../../.gitbook/assets/image%20%2883%29.png)

![](../../../../../.gitbook/assets/image%20%2878%29.png)

![](../../../../../.gitbook/assets/image%20%2874%29.png)

![](../../../../../.gitbook/assets/image%20%2882%29.png)

![](../../../../../.gitbook/assets/image%20%2870%29.png)

Thus as h -&gt; 0, sin\(h\)/h = 0, leaving us with dy/dx\(sinx\) = cosx

### Equations

![](../../../../../.gitbook/assets/image%20%2884%29.png)

## Spherical differentiation

There are some special cases, like these 2:

![](../../../../../.gitbook/assets/image%20%2875%29.png)

## Composite Functions

### Chain Rule

Used where there is a function, to the power of a function

**Formula**

![OR](../../../../../.gitbook/assets/image%20%2864%29.png)

![](../../../../../.gitbook/assets/image%20%2868%29.png)

**Example**

![](../../../../../.gitbook/assets/image%20%2872%29.png)

### Product Rule

Used for find the differentiation of 2 functions that multiply together

**Formula**

![OR](../../../../../.gitbook/assets/image%20%2862%29.png)

![](../../../../../.gitbook/assets/image%20%2881%29.png)

**Example**

![](../../../../../.gitbook/assets/image%20%2866%29.png)

### Quotient Rule

Used to find the derivative of 2 functions that are divided by one another

**Formula**

![OR](../../../../../.gitbook/assets/image%20%2863%29.png)

![](../../../../../.gitbook/assets/image%20%2877%29.png)

**Example**

![](../../../../../.gitbook/assets/image%20%2879%29.png)

## Numerical Methods

We can use MATLAB.



**Estimate for the derivative of a function**

![](../../../../../.gitbook/assets/image%20%2869%29.png)

**Example**

![](../../../../../.gitbook/assets/image%20%2865%29.png)

### General Rule

We approximate dy/dx using data points

![](../../../../../.gitbook/assets/image%20%2885%29.png)

### Using MATLAB

Something like this:

`X=[0,0.01,0.04,0.09 ...]`

`Xdiff = X(1, 2:end) - X(1, 1:end-1)`

