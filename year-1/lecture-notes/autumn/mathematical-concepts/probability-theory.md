---
description: Mathematical concepts lecture 7 - 19/10/2021
---

# Probability Theory

## Power set&#x20;

For a set $$S$$ the power set $$P(S)$$ is the set of all subsets of $$S$$ - including $$S$$ itself, and the empty set $$\emptyset$$

## Probability&#x20;

A way of describing things that _can_ happen, but without committing to whether they _will_ happen - and also without committing to precisely _how_

### Examples

What are the chances of rolling a total of 7 on two six-sided dice?

What are the chances of it raining in Brighton this week

### Sample spaces and events

#### Definitions

* $$\Omega$$: **Sample space** - a set of "elementary events" (i.e., very specific things that can happen)
* $$\omega \in \Omega$$: **Elementary event** - one very specific thing that could happen&#x20;
* $$E \in \Omega$$: An **event** (a set of specific ways, that make up ways that something more general could happen)

#### Typical examples

Outcome of throwing one die

$$
D=\{1,2,3,4,5,6\}\\\Omega=\{1,2,3,4,5,6\}
$$

### Probability Measure

**Concept:**&#x20;

* **A probability measure** is a mapping from 'events' $$E \in \Omega$$, to the probability that (an elementary event in) $$E$$happens

#### Definition

A probability measure is a function&#x20;

$$
P:P(\Omega)\rightarrow[0,1]\\E\mapsto P(E)
$$

... with some extra properties, eg $$P(\emptyset)=0, P(\Omega)=1$$



For $$P$$ to be a proper **probability measure**, the following conditions must hold:

* $$P(\emptyset) = 0$$
* $$P(\Omega) = 1$$
* For disjoint/exclusive events $$A, B \in P(\Omega)$$ - i.e.,  such that $$A \cap B = \emptyset$$ - we have $$P(A \cup B) = P(A) + P(B)$$



## Probability space

A **probability space** is a pair $$(\Omega, P)$$, made up of a sample space $$\Omega$$ and a probability measure $$P$$.

Some definitions consider a particular collection of events $$F \subset P(\Omega)$$ - an event space - and define a probability as a tuple space $$(\Omega, F, P)$$. But we will just take $$F = P(\Omega)$$

### Shorthand

We may write _e.g._ $$P(x < 5)$$ to represent the probability of some event $$E = \{x \in \Omega: x < 5\}$$, for some probability space $$(\Omega, P)$$.

## Probability of the complement

* Let $$A \subseteq \Omega$$ be an event
* Then $$A^C = \Omega \backslash A \dots$$or, equivalently: $$A \cup A^C = \Omega$$ and $$A \cap A^C = \emptyset$$
* Therefore, $$P(A) + P(A^C) = P(A \cup A^C) = 1 - P(A)$$

## Independence

**Definition:** Two events, $$A$$ and $$B$$ are independent if and only if $$P(A \cap B) = P(A) \cdot P(B)$$

_Not to be confused with A and B being disjoint or exclusive!_

## Bayes  Rule



$$
P(A|B)=\frac{P(B|A)P(A)}{P(B)}
$$

## Random Variables

A random variable is a function, from the sample space to some set $$S$$

### Example 1

**Flipping a coin**

$$
F:\Omega\rightarrow\{\text{Heads},\text{Tails}\}
$$



$$
\omega\mapsto (\text{in the situation described}\\\text{ by $\omega$ did the coin flip up \textbf{Heads} or \textbf{tails}?}
$$

## Variance



$$
\text{Var}(X)=\mathbb{E}([X - \mathbb{E}(X)]^2)
$$

## Expectation value



$$
\mathbb{E}(X)=\sum_{\omega \in \Omega}P(\{\omega\})\cdot X(\omega)
$$

## Standard Deviation



$$
\sigma_X=\sqrt{\text{Var}(X)}
$$

## Some properties of Expectation and Variance

For **any** random variables $$X_i$$(for $$i=1,\dots,n)$$:&#x20;



$$
\mathbb{E}\biggl(\sum^n_{i=1} X_i\biggl)=\sum^n_{i = 1}\mathbb{E}(X_i)
$$

This is known as the additivity of Expectation



## Bernoulli Process

A bernoulli process is a process with independant binary outcomes, such as coin flips

$$
\Omega=\{0,1\}^n=\{(\omega_1,\dots,\omega_n):\omega_i\in \{0,1\}\}
$$

### Bernoulli distribution

Distribution of a single binary outcome for any choice of $$p$$



$$
P(\{\omega_i=1\})=p
$$

## Covariance

Covariance characterizes the relationship between **two random variables**, $$X$$, and $$Y$$, how much they "**co-vary**".



$$
X:\Omega\rightarrow \mathbb{R} ~\text{and}~Y:\Omega \rightarrow \mathbb{R}
$$

