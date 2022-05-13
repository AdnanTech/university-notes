---
description: 18/10/2021
---

# The correctness of algorithms

## The problem

## Assertions

Assertions are mathematical statements about variables at some specific checkpoint in a program. An assertion is valid if it is true of the program **every time** control passes the checkpoint.&#x20;

### Important assertions

**Initial assertions**: Capture requirements on legal inputs

**Final assertions**: Determines properties of data output

**Loop assertions**: Difficult to assign, must be true **every** time control goes through the loop

### Assigning valid assertions

In order to assign valid assertions, we can use semi-automatic software solutions, however, this course typically uses **informal** mathematical reasoning, such as loop invariance theorems.&#x20;

#### Example

![An example algorithm with valid assertions](<../../../../.gitbook/assets/image (195) (1).png>)

```
ptr <- 1
cmax <- A[ptr]
// assert: cmax = A[1]
while ptr != n do
    // assert: cmax is the largest element in A[1..ptr]
    ptr <- ptr + 1
    if A[ptr] > cmax then 
        cmax <- A[ptr]
// assert: ptr = n and cmax is the largest element in A[1..ptr]       
return cmax
```

### Warnings

* Assertions say nothing about termination
* Final assertion describes properties which are true _if_ the program terminates&#x20;
* Separate reasoning needs to be done to ensure termination
  * Usually requires some quantity which decreases each time round the loop
  * Sometimes involves the manner in which this quantity decreases&#x20;
* Never write a for loop without knowing why it will terminate, for ever possible inputs&#x20;



## Reasoning about programs

### Floyd Hoare logic

We write `{pre} C {post}` where pre is a mathematical assertion - the precondition, C is some program code, and post is another mathematical assertion, known as the post condition.&#x20;



## Examples
