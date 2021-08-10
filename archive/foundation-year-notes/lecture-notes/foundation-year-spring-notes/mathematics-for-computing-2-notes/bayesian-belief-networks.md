# Bayesian Belief Networks

Bayes Networks, also known as Bayesian Belief Networks, allow us to represent the casual relationships between events, for example, studying and a good grade.

The idea of casuality indicates that studying causes a good grade, but a good grade is not always represented with studying. The links determine whether they are conditionally dependant, or conditionally independant.

We can also drive inference from **cause to effect using the joint probability rule**. Or we can go from **effect to cause using the Bayes rule**.

## Formulae \(Bayes Rule\)

![](../../../../../.gitbook/assets/image%20%28166%29.png)

## Belief Networks

The idea of belief networks, as stated earlier, is to show casual relationships using a graph and probability distribution.

### Example 1

Going back to the idea of studying leading to a good grade, but good grades not always being equal to studying, we can represent it like so, with the circles being **nodes** that represent the probablity distribution

![](../../../../../.gitbook/assets/image%20%28156%29.png)

This can also be summed up, which was shown in [discrete probability.](discrete-probablity.md#summing-away-variables) For example, if we wanted to work out the probability that we study hard and get a B:

![](../../../../../.gitbook/assets/image%20%28146%29.png)

Using P\(G, S\) = P\(G\|S\) . P\(S\), we can see the odds are 0.2.

**General Equation:**

![](../../../../../.gitbook/assets/image%20%28144%29.png)

### Example 2

* P\(R\) – the probability that it is raining
* P\(S\) – the probability that a sprinkler is on or off
* P\(W\) – the probability that the grass is wet

Therefore the grass can be wet either because it is raining, or because the sprinkler is on, or both. But, the sprinklet is only on depending on whether it's raining.

![](../../../../../.gitbook/assets/image%20%28142%29.png)

Because the rain causes the sprinkler to be on or off, it means that rain must add up to one, however, the reverse is not true. 

If the sprinkler is on, what is the probability that it is raining, this brings us to the most important point: **the Joint Probability is used for working out the probability in the forwards direction, to go backwards, we use the bayes rule.**

Therefore, solving \(If the sprinkler is on, what is the probability that it is raining\):

![](../../../../../.gitbook/assets/image%20%28179%29.png)

