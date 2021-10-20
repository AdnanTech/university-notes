# Worksheet 3

Write an algorithm that will decide if two arrays (of the same length) are equal.&#x20;

```
Input: Arrays A[1...n], B[1...n]
Output A = B

for i <- 1 to n
    for PTR <- 1 to n
        if A[i] == B[PTR]:
            break
        if PTR == n:
            return false
return true
```
