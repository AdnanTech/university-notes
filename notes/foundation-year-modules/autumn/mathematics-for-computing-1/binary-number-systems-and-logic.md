# Binary Number Systems and Logic

**Every number system starts at base zero, which is the actual digit one**

![](../../../../.gitbook/assets/image%20%28100%29.png)

Binary is base 2 whereas denary is base 10.

Example of Binary:

![](../../../../.gitbook/assets/image%20%2898%29.png)

Numbers are digits, in binary they are called bits

You can convert denary to binary with arithmetic calculations.

log2\(number\) will be equal to the number of \(2^bits\) bits - 1

## Arithmetic calculations with binary

### Addition

![](../../../../.gitbook/assets/image%20%2887%29.png)

### Subtraction

* Method 1, is borrowing numbers, using the same technique used in denary subtraction by hand. so if you borrow a 1 for a 0, it turns to 10, being 2. Then the 1 that was borrowed has to pay back. either the top 1 borrowed from becomes zero, or the number underneath the 1 that was borrowed from increases by 1. The situation will depend on who pays back, usually it does not matter. the golden rule is \(decrease the top after borrowing or increase the bottom after borrowing - both for the column on the left of the borrower\).
* Method 2 is essentially just adding a number and a negative number together

Subtraction is the exact same in binary as in denary. You borrow to find 2, and then subtract 1, if you are not doing 1-0  or 0-0.

![](../../../../.gitbook/assets/image%20%2888%29.png)

### Multiplication

So whats happening here is that we take each bit from the bottom row, multiply it by the top row, and shift the row over. We do this until 0, then 1, then 0, then 1 are all multiplied by the top.

Afterwards, we add the bits together to get the result

![](../../../../.gitbook/assets/image%20%28101%29.png)

### Doubling Binary Numbers

* There is also an easy way of multiplying by 2 \(10 subscript 2 is binary\)
* Just shift the binary number to the left, filling in spaces with 0’s
* E.g:111 x 10 = 11101110 x 10 = 11100
* Analogous to moving the decimal point in denary

## Hexadecimal

![](../../../../.gitbook/assets/image%20%2897%29.png)

![](../../../../.gitbook/assets/image%20%2894%29.png)

![](../../../../.gitbook/assets/image%20%2893%29.png)

![](../../../../.gitbook/assets/image%20%2889%29.png)

![](../../../../.gitbook/assets/image%20%2899%29.png)

![](../../../../.gitbook/assets/image%20%2895%29.png)





