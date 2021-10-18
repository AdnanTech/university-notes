# Homework 2

> The following algorithm will sort an array A into ascending order. Consider using this algorithm on an array A = \[8, 1, 7, 5]. Write the array A after each iteration of the outer For-loop.

```
Input: Array A[1...n]
Output: Array A sorted

for i <- 1 to (n - 1) do
    MINPTR <- i
    // maintains A[1...i] sorted
    for j <- (i + 1) to n do
        // finds smallest item in A[i...n]
        if A[j] < A[MINPTR] then
            MINPTR <- j
        A[i] <-> A[MINPTR] //swap items
    return A
```

```
A = [8, 1, 7, 5]
    [1, 8, 7, 5] // first iteration
    [1, 5, 7, 8] // second iteration
    [1, 5, 7, 8] // third iteration
```

> Write an algorithm to decide if an array A\[1...n] is sorted in ascending order. 

```
Input: Array A[1...n]
Output: Boolean, true if A is in ascending order.

i <- 1
j <- i + 1
while i < j do
    i <- i + 1
    j <- i + 1
    if j == n
        return true
return false
```

```
// PYTHON
def ascending(A):
    i = 0
    j = i + 1
    while A[i] < A[j]:
        i = i + 1
        j = i + 1
        if j == len(A):
            return True
    return False
```
