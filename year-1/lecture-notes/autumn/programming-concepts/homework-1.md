# Homework 1

Write an algorithm that inputs an arrayA\[1...n]and returns the same array with the elements in reverse order. Here are 3 examples: the reverse of the array\[1,2,3,4]is\[4,3,2,1], the reverse of the array\[3,0,7,9,2]is\[2,9,7,0,3]and the reverse of\[3]is\[3]. Your algorithm should work in-situ(i.e. an in-place algorithm that does not use any other array)

```
INPUT: an array A[1...n]
OUTPUT: the same array in reverse order

for i <- 1 to (n/2):
    temp <- A[i]
    A[i] <- A[n - i + 1]
    A[n] <- A[i]
```

Write down an algorithm in pseudo-code which returns the sum of all the even numbers in an arrayA\[1. . . n]. 

```
INPUT: an array A[1...n]
OUTPUT: sum of all even numbers in input array

for i <- 1 to n:
    if A[i] % 2 == 0:
        sum += A[i]
```
