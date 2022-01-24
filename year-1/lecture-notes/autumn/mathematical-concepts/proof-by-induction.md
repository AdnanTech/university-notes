---
description: '07/10/2021 - TODO: refactor notes'
---

# Proof by Induction

## Predicates

A predicate $$P(N)$$is a or statement which can either be **true** or **false**, for an argument $$n$$. For example, $$P(n):$$"n is divisible by either 2 or 3"

## Proving a 'Universal'

We consider some **predicate** $$P(n)$$for an argument $$n \in \mathbb{N}$$. For example, $$P(n): n^3 - n$$is divisible by 3

## Mathematical induction

* Show that $$P(n) \rightarrow P(n+1)$$
* Show that $$P(0)$$is true&#x20;

If $$P(0)$$ , and $$P(n) \rightarrow P(n+1)$$for all $$n \in \mathbb{N}$$then $$P(n)$$for all $$n \in \mathbb{N}$$.

In mathematical notation,

$$
P(0) \& (\forall n \in \mathbb{N}: P(n) \rightarrow P(n + 1)) \rightarrow P(n) \in \mathbb{N}
$$

### Example 1

* $$P(n): n^3 - n$$is divisible by 3
* Case $$n = 0: 0^3 - 0 = 0$$is divisible by 3
* To prove that for any $$n \in \mathbb{N}, P(n) \Rightarrow P(n+1)$$:
  * First, suppose that $$P(n)$$is true. This is known as the induction hypothesis&#x20;
  * Required to show that it follows that $$P(n+1)$$is true.&#x20;

That is, we need to show that $$(n + 1)^3 - (n + 1)$$is divisible by three



### Example 2

Prove that&#x20;

$$
P(n): \sum^n_{k=1}(2k-1)=n^2
$$

$$
P(0): \sum^0_{k=1}(2k-1)=0^2
$$

#### Induction step

Suppose that $$P(n)$$holds for some $$n \in \mathbb{N}$$

$$
P(n+1):\sum^{n+1}_{k=1}(2k-1)=(2(n+1)-1)+\sum^n_{k=1}(2k-1)\\
=(2n+2-1) + n^2\\
=n^2+2n+1\\
=(n+1)^2
$$

### Example 3

#### Claim: (for $$q\neq1$$)

$$
P(n): \sum^{n}_{i=0}q^i=\frac{1 - q^{n+1}}{1-q}
$$

#### Proof:

Base case: $$n = 0$$

$$
\sum^0_{i=0}q^0=1=\frac{1-q^1}{1-q}
$$

Induction step:&#x20;

**Hypothesis:** $$\sum^{n}_{i=0}q^i$$for some $$n\in \mathbb{N}$$

**Then:**&#x20;

$$
\sum^{n+1}_{i=0}q^i=\sum^{n}_{i=0}q^i+q^{n+1}=\frac{1-q^{n+1}}{1-q} + q^{n+1} \cdot \frac{1-q}{1-q}\\
=\frac{1-q^{n+1}+q^{n+1}-q^{n+2}}{1-q} \\
=\frac{1-q^{n+2}}{1-q}\\
$$

