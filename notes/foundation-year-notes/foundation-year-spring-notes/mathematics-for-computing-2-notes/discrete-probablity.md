# Discrete Probablity

Distributions are ways of showing probabilities of events, essentially the chances of specific outcomes.

These can be **real valued,** for example height or salary. Or they can be **discrete valued**, like a true or false or range of values.

## Formulae for Joint Distributions

![](../../../../.gitbook/assets/image%20%28172%29.png)

## Uniform Distribution

In discrete probability, 0 means it does not happen, and 1 means it will happen every time, considering a coin, this can be represented in math like so:

* P\(head\) = 0.5
* P\(tails\) = 0.5

Therefore the sum of all outcomes is 1.

This can also be represented as a bar chart, these are called **histograms**. A histogram for a dice would look like:

![](../../../../.gitbook/assets/image%20%28141%29.png)

From the image, we can deduce it is a **uniform distribution**. The probability of each outcome would be 1/N, where N is the number of possible outcomes.

## Distribution Tables

* P\(X\) represents the probability of a distribution
* P\(X=x\) is the probability that X has a specific value x
* P\(X, Y\) represents a joint probability distribution
* P\(X=x, Y=y\) is the probability that X has a specific value x and Y has a specific value y

### Uniform Distributions

For P\(X\), so one dependant variable:

![](../../../../.gitbook/assets/image%20%28163%29.png)

### Joint Discrete Distributions

For P\(X, Y\):

![](../../../../.gitbook/assets/image%20%28186%29.png)

### Summing Away Variables

Using this information, and putting in some example variables, we can work things out, for example, using the table below, we can find P\(X = red\), using the formula:

![](../../../../.gitbook/assets/image%20%28150%29.png)

![](../../../../.gitbook/assets/image%20%28158%29.png)

The probability of P\(x = red\)  = 0.3

## Joint Probability

* P\(X,Y\) is a joint probability
* P\(X,Y\) = P\(X\|Y\) P\(Y\)
* Joint probability of X and Y is the Probability of X given Y \* Probability of Y
* Depends on whether X and Y are conditionally dependent or independent of each other

### **Conditional Dependence**

Is where the variables depend on each other, for example: _if the weather is rainy today, then there is a probability that it will be rainy tomorrow_:

P\(X=rainy today, Y=rainy tomorrow\) = 0.6

_What’s the probability that it will rain tomorrow?_ Depends on whether it is rainy today: `P(X=rainy today, Y=rainy tomorrow) = P(Y=rainy tomorrow | X=rainy today ) * P(X = rainy today)`

### Conditional Independence

The idea of conditional independence is where the variables do not depend on one another. A good example of this is flipping a coin, where:

* `P(f1 = heads, f2 = heads) = 0.25`
* `P(f1=heads,f2 = heads) = P(f2 = heads|f1 = heads) *` _`P(1 = heads)`_
* _But `P(f2 = heads|f1 = heads) = P(f2 = heads)`_
* _So: `P(f1=heads,f2 = heads) = P(f2 = heads)`_  `P(f1 = heads)`

