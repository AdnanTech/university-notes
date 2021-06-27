# Bionomial Distribution

## Definition

A **binomial distribution** can be thought of as simply the probability of a SUCCESS or FAILURE outcome in an experiment or survey that is repeated multiple times. The binomial is a type of distribution that has **ONLY** **two possible outcomes.**

## Formula

![](../../../../.gitbook/assets/image%20%28140%29.png)

Where \(n x\) is \(n C x\), and ! means factorial \(0! = 1\)

`X ~ Bin (n, p)` is used to denote any binomial calculations. This is written before any probability calculations, where n is the number of trials, and p is the probability of success of a trial.

![](../../../../.gitbook/assets/image%20%28137%29.png)

![Where r is the number of trials](../../../../.gitbook/assets/image%20%28134%29.png)

**This is the formula for an exact number:**

![](../../../../.gitbook/assets/image%20%28178%29.png)

### **Mean and Variance**

![](../../../../.gitbook/assets/image%20%28143%29.png)

**Where E\(X\) is the expected value, aka the mean. And Var\(X\) is the variance.**

## **Example**

For exactly 3 heads to be obtained in 5 coin flips:

![](../../../../.gitbook/assets/image%20%28145%29.png)

Therefore, using the 10

![](../../../../.gitbook/assets/image%20%28138%29.png)

## Permutations

![](../../../../.gitbook/assets/image%20%28182%29.png)

## **Pascal's Triangle**

**Where C is Pascal's Triangle**

![](../../../../.gitbook/assets/image%20%28139%29.png)

Note that:

* ! means factorial
* 1! = 1
* 0! = 1

## **Bernoulli Distribution**

The bonimal distribution is similar to the Bernoulli distribution. A Bernouilli trial: If there is **only 1 trial** with probability of success p and probability of failure 1-p, this is called a Bernouilli distribution. \(special case of the binomial with n=1\)

![](../../../../.gitbook/assets/image%20%28136%29.png)

For Bernouilli \(n=1\):

* E\(X\) = p
* Var \(X\) = p\(1-p\)

