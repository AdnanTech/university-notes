# Limits

## A looser notation of limiting behavior

**Asymptotic analysis **provides a formal way to descrie hand wavy comparisons of functions

* Only considering functions up to leading terms (ignoring the difference between x^2 and x^2 + 2x)
* Even ignoring scalar factor differences! (Brushing aside the difference between x^2 and 5x^2)

### Definition&#x20;

There is an $$\alpha \in \mathbb{R}$$ and $$N \in \mathbb{N}$$ such that for all $$x > N:$$

$$
O(g)=\{f:\mathbb{N}\rightarrow\mathbb{R}:0\leq|f(x)|\leq\alpha \cdot g(x)\}
$$

### Asymptotic growth of polynomials

Despite the fact that x^2 + 2x > x^2 for all x > 0: we may show that $$x^2 + 2x \in O(x^2)$$

#### Proof

* For $$x > 0$$,

$$
\frac{x^2 + 2x}{x^2}=1+\frac{2}{x}\rightarrow 1+0=1
$$

... as the ratio $$\frac{x^2 + 2x}{x^2}$$**converges, **it is in particular bounded

* We also have $$x^2 + 2x \in O(x^3):$$ for $$x > 0$$,



$$
\frac{x^2+2x}{x^3}=\frac{1}{x}+\frac{2}{x^2
$$

