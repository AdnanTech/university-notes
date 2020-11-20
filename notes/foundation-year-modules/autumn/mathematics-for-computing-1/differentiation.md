# Differentiation

## Differentiation

Differentiation belongs to calculus, and touches on rate of change. Differentiation, was co-invented by Isaac Newton and  Gottfried Wilhelm Leibniz. The derivative is the slope of a tangent of an arbitrary slope, in geometrical terms. This is where a straight line can be drawn on a point of a curve, and allows for you to find a gradient at a specific point.

Derivatives have applications throughout all of nature, image edges, velocity, fluctuations in interest rates, spikes in noisy audio data, market changes \(bull and bear\) and more.

Differentiation also relates to units. Take a graph of distance against time, distance is on the y axis, and time is on the x axis, so dy/dx = m/s = ms^-1

To differentiate, you make the equation equal to zero, and then you follow the formula.

## Terminology

* DeltaT -&gt; 0 = in the limit as deltaT tends towards zero
* Delta \(triangle\) = \(small\) change, so
* Deltax = \(small\) change in x
* d = infinitesimally small change \(ideally the minimum change, closest to zero we can find\)
* dx = infinitesimally small change in x
* dy/dx = the derivative, the instantaneous rate of change in y relative to x
* f'\(x\) is the same as dy/dx \(pronounced f prime x\), belonged to lebneiz, whereas dy/dx was the style that belonged to Isaac Newton

## Lecture 2 Notes

The general form of a gradient for a straight line:

![](../../../../.gitbook/assets/image%20%2855%29.png)

As a graph, it can be represented like so:

![](../../../../.gitbook/assets/image%20%2854%29.png)

This equation can be applied to curves, with the derivative

![](../../../../.gitbook/assets/image%20%2860%29.png)

## Proof

![](../../../../.gitbook/assets/image%20%2853%29.png)

## Stationary Points

When rate of change = 0, we have a “level” or flat point in a function​, We call this a stationary point for the function​, We could find these points through accurate graph drawing.

The stationary point is where the derivative is equal to zero. You differentiate, and sub in the original x solutions.

## Derivative on linear functions

![](../../../../.gitbook/assets/image%20%2858%29.png)

## Derivative of a constant line

![](../../../../.gitbook/assets/image%20%2856%29.png)

## Solving a cubic's stationary points

![](../../../../.gitbook/assets/image%20%2859%29.png)

## Equations

### General differentiation

![](../../../../.gitbook/assets/image%20%2851%29.png)



### Trigonometry differentiation equations

![](../../../../.gitbook/assets/image%20%2852%29.png)

### Common derivatives

![](../../../../.gitbook/assets/image%20%2848%29.png)

## Solving using numerical methods

* Pick random x and y points from the graph
* find the difference between d\(change in\) y \(y2 - y1\) and d\(change in\) x \(x2 - x1\) of two points clos to each other
* find dy/dx
* This will gave a gradient, \(dy/dx\) thus the differential is found, if zero, stationairy point
* accuracy will be increased if the points are closer together \(diff in x and diff in y is extremely small\)

![for the equation 3x^2-6x-1](../../../../.gitbook/assets/image%20%2861%29.png)

### Smoothing graphs with rough gradients

To remove the spike values, we just set a filter on the gradient so it excludes the anomalies in the graph.

We can do this adding a new column, with a formula saying =if\(gradient&gt;threshold, "anomaly", 0\)

Doing this, we can then estimate the values where there in anomaly, based on the data around it, using the mid point of the two values above and below the anomaly.

The excel way to do this, is to create a new column that has the corrected values in, to say if there in error present, correct it, else leave it as the actual value.

The assumption we are making with this method, is that the points either side of the corrected values are also correct, there might need to be a spike in the data, what if it's a heartbeat? This is represented throughout life too, we make assumptions, and assume truths based on those assumptions.



