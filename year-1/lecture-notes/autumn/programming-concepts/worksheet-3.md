# Worksheet 3

Write an algorithm that will decide if two arrays (of the same length) are equal.&#x20;

```
Input: Arrays A[1...n], B[1...n]
Output A = B

i <- 1
j <- 1

while A[i] == B[j]
    for j <- 1 to n
        if A[i] != B[j]
            return false
    if i == n and j == n
        return true
 
return false
```
