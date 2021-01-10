# Logic and Combinational Logic

## Logic

* A logic gate an implementation \(usually with an electronic circuit, now more commonly called chips\) of a Boolean function
* A Boolean function is one that uses just two values \(just like in programming\)
  * TRUE / 1 / ON
    * High voltage
    * Low resistance
    * Similar to an operational amplifier
  * FALSE / 0 / OFF
* A Boolean function may have 1 or more inputs, and exactly 1 output

These originate from the transistor, made in 1957, to replace glass vaccuum tube transistors. Smaller size, faster, cheaper etc.

Chips, including the transistors on the chip, are made from silicon. The choice of material is due to it's conductivity, but mainly its abundance on earth.

The fastest way to know the maximum possible number outputs to a logic gate is the number of inputs \(A,B,C = 3\) to the power of 2. So for ABC input, max combinations is 2^3

The outputs are also in 4 pairs, 2 pairs, and then binary, for example:

![](../../../../.gitbook/assets/image%20%28117%29.png)

## The logic gates

Logic gates can be bought in chip packages, where are are 2, 4 6 or 8 gates on the chip. Each chip was a boolean function.

### AND gate

![](../../../../.gitbook/assets/image%20%28103%29.png)

### NAND gate

NAND is special because any boolean function can be implemented by using a combination of **NAND** gates. This property is called functional completeness. Essentially, every gate can be represented as NANDs gates. So that's why we use NAND gates in devices.

Usually, when we design chips, the only purpose of every other gate, is to help with the design. During manufacturing, we convert all the gates to NAND gates, and devise a chip based off of that. Hence all  major devices use NAND gates

![](../../../../.gitbook/assets/image%20%28106%29.png)

### OR gate

![](../../../../.gitbook/assets/image%20%28102%29.png)

### XOR gate

![](../../../../.gitbook/assets/image%20%28109%29.png)

### NOT gate

![](../../../../.gitbook/assets/image%20%28107%29.png)

### Cheat Sheet

![](../../../../.gitbook/assets/image%20%28108%29.png)

### Truth Table

![](../../../../.gitbook/assets/image%20%28112%29.png)

### Logic Gate expressions

![](../../../../.gitbook/assets/image%20%28114%29.png)

### Boolean expressions

Simplifying expressions, we can simplify the expression above

![](../../../../.gitbook/assets/image%20%28111%29.png)

Which can also be represented with logic gates

![](../../../../.gitbook/assets/image%20%28110%29.png)

## Excel

We can also represent Truth tables in Excel, with a formula of =AND\(cell1, cell2\), replacing AND with the appropiate gate.

## Boolean written expression

`X = (A AND B AND C) OR (A AND B) OR (A AND C) OR (B AND C)` can be written as: `X = ABC + AB + AC + BC`

## Simplifying Laws

Booleans can be simplified, with the same laws used in college:

* **A + ~A = 1**
* **A + ~A.B = A + B**
* **1.A = A**
* **A.\(B + C\) = A.B + A.C \(distribution\)**
* **A.B + A.C = A.\(B + C\) \(factorisation\)**

Where: . is AND, + is OR and ~ is NOT 

## Karnaugh Maps

Karnaugh maps are a method to display a truth table, these help us solve electronic circuits, to solve logic problems. The idea is that we can **simplify boolean expressions** using a rectangle/square table, rather than long columns. For example:

![](../../../../.gitbook/assets/image%20%28104%29.png)

### Gray Code form

In gray code form, only 1 bit changes at a time. Gray form itself in maths means that only one piece of information changes at a time, being the bits. It has significance in karnaugh maps because in gray code order, because to convert binary data in columns to a karnaugh map, is it best converted when the binary data is in gray code form.

Gray code form also underpins how we represent truth tables, note how only one bit changes at a time, like so:

![](../../../../.gitbook/assets/image%20%28119%29.png)

### Converting Binary Data to Karnaugh maps

it maps one to one, using the framework discussed in gray code form. For every binary data set, there is a karnaugh map, and vice versa

![](../../../../.gitbook/assets/image%20%28120%29.png)

### Grouping rules

There are some simple groupign rules for squares/rectangles on a karnaugh map

* We can only group in base 2's \(1, 2, 4, 8, 16\)
* They cannot be diagonal
* They CAN wrap around the box \(bottom down and back to the top of the diagram and vice versa\)
* They must be as big as possible
* They can only wrap around 1s

### Example

Consider this karnaugh diagram, we have 2 boxes, as large as possible.

![](../../../../.gitbook/assets/image%20%28121%29.png)

The red and blue boxes are seperate, represent the sum of products expression together. So from the diagram:

* The red box, has a B constant, as well as a D constant, therefore the red block is B AND D
* The blue box, has a A constant, and not C and not D are constant, therefore the block is A AND \(NOT C\) AND \(NOT D\)

T**hese boxes can then be combined and seperated with an OR**, so the red and the blue block, the output, can be represented as \(A . ~C . ~D\) + B.D

## Representing all gates as NAND

The 3 most core logic gates, NOT, AND, OR can be represented as a group of NAND gates. And these are used in DESIGN. NAND gates are used in MANUFACTURING.

![](../../../../.gitbook/assets/image%20%28113%29.png)

