---
description: 26th October 2021
---

# Statistics

## Statistics vs. Probability theory

In statistics, _we do not know _the underlying probability space $$(\Omega, P)$$ - which is where probability theory starts. **Instead **we have some limited information (data points, samples) of some system. However, both are related. **We use probability theory to make sense of statistics. **

Experimental data is used to estimate a model in order to predict future trials of the experimental data.&#x20;

![](<../../../../.gitbook/assets/image (196).png>)

## Statistical Measures

### Mean&#x20;

The mean of a set of observations: $$\{x_i: i = 1, \dots, n\}$$ is defined as follows:

$$
\bar{x}=\frac{1}{n}\sum^n_{i=1}x_i
$$

The mean is also commonly refered to as the average

### Centeral limit theorem

For $$n$$ independent, identically distributed (i.i.d) random variables $$x_i~$$("samples"), with expectation $$\mu~$$and variance $$\sigma^2$$: the distribution of

$$
T_n=\sum^n_{i=1}x_i
$$

has mean $$n\mu~$$and variance $$n\sigma^2$$ (by additivity)



In particular: the sample mean

$$
\bar{x}_n=\frac{T_n}{n}=\frac{1}{n}\sum^{n}_{i=1}x_i
$$

is itself a random variable, with expectation value $$\mu~$$(i.e. $$\mathbb{E}(\bar{x}_i=\mu)~$$and standard deviation $$\frac{\sigma}{\sqrt{n}}$$

### Standard Deviation&#x20;

