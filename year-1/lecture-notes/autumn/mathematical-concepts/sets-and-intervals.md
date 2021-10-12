---
description: Mathematical Concepts lecture - 12/10/2021
---

# Sets and Intervals

## Summary

* Sets
* Set relations 
* Set operations
* Set notation

## Sets

Sets are a collection of things, typically numbers. The things in the sets are refered to as the **elements **of the set. 

The general notation for a set is as follows:



$$
\{0,1,2,3\}\\\mathbb{N} = \{0,1,2,3,\dots\}
$$



### Set notation

#### Descriptors with a condition



$$
S=\{x\in X:P(x)\}
$$

This means that the set contains only elements of the set $$X$$where a predicate $$P(x)$$holds. 

#### Formulas over a range



$$
f(x) = x * e^{2 pi i \xi x}
$$

#### Examples

* Perfect squares $$S=\{n^2: n \in \mathbb{N}\}$$
* Composite numbers $$C = \{a \cdot b: a, b \in \mathbb{N} \land  a,b > 1\}$$
* Prime numbers $$P = \{n \in \mathbb{N}: n \not \in \mathbb{C} \land n > 1\}$$
* The empty set $$E = \{n \in \mathbb{N}: n \in C \land n < 4\} = \{\}$$

### Venn Diagrams

Sometimes it helps to visualise sets within venn diagrams

### Set relations

* $$A \subseteq B: A~$$is a subset of $$B$$
* $$A \subset B: A$$ is a proper subset of $$B$$

### Set operations

* Unions $$A \cup B = \{x: (x \in A) \lor (x \in B)\}$$
* Intersections $$A\cap B = \{x: (x \in A) \land (x \in B)\}$$
* Set subtraction $$A~\backslash~B = \{x \in A: x \not \in B\}$$
* Complements $$A^C = U~\backslash~A$$
* Cardinality $$A = \{1,2,3,4\}, |A| = 4$$

### Infinite cardinalities

We can extend **cardinality** to infinate sets. We say that $$|\mathbb{N}|\geq|\mathbb{Z}|$$if we can match each element of $$A$$with a **distinct **element of $$B$$.

$$|{\mathbb{N}}|=: \aleph_0$$ ("aleph nought" - countable infinity)

## Intervals

Intervals are a special type of **subsets of **$$\mathbb{R}$$. For $$x,y \in \mathbb{R} \land x < y$$:  the resulting interval is **closed**, meaning it contains all numbers between $$x$$ and $$y$$ 

$$[x,y] = \{z \in \mathbb{R}: x \leq z \leq y \}$$

Open intervals are intervals between $$x$$and $$y$$ but not including the boundries

$$(x, y) = \{z \in \mathbb{R}: x < z < y\}$$

Neither are the same as $$\{x, y\}$$, which is a set only containing $$x$$and $$y$$

#### Half open intervals



$$
[x, y) = \{z \in \mathbb{R}: x \leq z < y\}\\(x,y] = \{z \in \mathbb{R}:x < z \leq y\}
$$





