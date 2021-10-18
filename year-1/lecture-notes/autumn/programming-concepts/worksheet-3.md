# Worksheet 3

Write an algorithm that will decide if two arrays (of the same length) are equal. 

```
Input: Arrays A[1...n], B[1...n]
Output A = B

for i <- 1 to n
    PTR <- 1
    while A[i] != B[PTR] do:
        if B[PTR] = n:
            return false
        PTR <- PTR + 1
return true
```
