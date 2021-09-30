---
description: What is a number?
---

# Number Sets

## ℕ - Natural Numbers

ℕ stands for a **natural** number. 

A natural number is any number that  
 may be obtained from 0, by applying the “**successor function**” `[S(n) = n + 1]` a finite number of times.

If 0 is not included, one might write N\_+ … or more often: Z\_+. However, in this course, we DO include zero as a natural number.

This encapsulates {0,1,2,3...} as well as the operations \( /, \*, +. - \[Where \* is a dot in the middle\]\). A general rule of thumb is that if you  add or multiply two natural numbers, the result is another natural number.

ℕ is closed under addition and multiplication”. ℕ is not closed under subtraction or division: 3−5 ∉ ℕ and 1/3 ∉ ℕ.

## ℤ - Integers

ℤ stands for **integers.** This involves { …, -2, -1, 0, 1,2, … }. Unlike ℕ, the integers ℤ are closed under subtraction, because it contains negative numbers.

**There is no ‘first’ integer**, which gives you the rest by applying the successor function; and the sum / product of two numbers, can be smaller than one or both of them.

## ℚ - Rational

ℚ stands for **rational** numbers, so fractions. ℚ is all numbers that can be written in the form 𝑎/𝑏, where 𝑎 and 𝑏 are integers: 𝑎 , 𝑏 ∈ ℤ \(but 𝑏 ≠ 0\).

𝑎 = “numerator”, 𝑏 = “denominator” Unlike ℤ, the set ℚ is closed under division \(so long as 𝑏 ≠ 0\).

Unlike ℤ, the set ℚ is closed under division \(so long as 𝑏 ≠ 0\). Unlike ℕ and ℤ, ℚ has **no successor function**: Between any two rational numbers there is another.

**ℚ still has an ordering:** for any 𝑎 ≠ 𝑏 ∈ ℚ : 𝑎 &lt; 𝑏 or 𝑏 &lt; 𝑎

### 

## ℝ – **Real** numbers

ℝ represents any tangible number, meaning it excludes imaginary numbers such as infinity or √-1.

A Real Number can have any number of digits on either side of the decimal point, so 1/3 is considered a Real Number despite having an infinite number of digits on the right of the decimal point.

## ℂ – **Complex** numbers

## Symbols of Logic

* ⇒ means “**implies**”
  * **𝑎 &gt; 5 ⇒ 𝑎 &gt; 3** 
* In general, the **opposite need not be true**
  * **𝑎 &gt; 3 ⇏ 𝑎 &gt; 5**
* If both directions are true, it’s called **equivalent**
  * **𝑎 = 3 ⇔ 2𝑎 = 6**

## Proof using the contra-positive

Proof there is no successor function for Rational Numbers:

If you have 2 rational numbers, x and y, where y is the next number in the sequence x, y, z. For this to be true, x &lt; y, therefore there is no successor function?

**Lemma. "x^2 is even" implies "x is even" for x ∈ ℕ**.

**Proof:**

Assume x is odd, i.e., x = 2n + 1 for n ∈ ℤ.

Then, x^2 = \(2n + 1\)^2 = 4n^2 + 4n + 1  
                                        = 2\(2n^2 + 2n\) + 1

Therefore, x^2 is odd  
**x is odd ⇒ x^2 is odd**

