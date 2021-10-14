# Worksheet 2

```
// using bounded iteration...

INPUT: an array A[1...n] with more than 1 element
OUTPUT: A[1...n] where all elements shifted one place to the left

temp <- A[i]
for i <- i to n - 1:
    A[i] <- A[i+1]
A[n] <- temp
return A
```

```
// using a for loop...

INPUT: an array of numbers A[1...n]
OUTPUT: returns the sum of all numbers in A

sum <- 0
for i <- 1 to n:
    sum += A[i]
return sum

// using a while loop...

INPUT: an array of numbers A[1...n]
OUTPUT: returns the sum of all numbers in A

sum <- 0 
i <- 1
while i <= n:
    sum <- sum A[i]
    i <- i + 1
return sum
```

```
// using bounded iteration...

INPUT: a non empty array A[1...n]
OUTPUT: average of elements in A

count <- 0
sum <- 0

for i <- 1 to n:
    sum <- sum + A[i]
    count <- count + 1
return sum / count
```

```
// Some code

INPUT: Array A[1...n], 
OUTPUT:
```
