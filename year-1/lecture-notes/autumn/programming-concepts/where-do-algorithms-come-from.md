# Where do algorithms come from?

## **Developing in Algorithm**

1. Understand the problem
2. Devise a plan for solving the problem
3. Carry out the plan
4. Evaluate the solution for accuracy

Steps are not always sequential, however _1 always comes first. But during 3, you may realise that 1 is not achieved or 2 is in incorrect_.

## Problem Solving

Two main methods to solve a problem, top-down and bottom-up.

### Top-Down

1. Don't solve the entire problem
2. Reduce problem into sub-problems
3. Tackle sub-problems
4. Eventually end up with smaller trivial problems

These steps are not always sequential also, as reduction into sub-problems may not work, or the sub problem could also possibly be even harder to solve than the larger problem it belonged to.

### Bottom-Up

1. Think directly about the problem itself
2. Examine simple instances
3. Solve trivial instances of the problem
4. Research algorithmic solutions to similar problems in literature
5. Try to understand intuitive mechanisms used in 3
6. Try to extend 3 to slightly more complicated instances
7. Get an idea for general algorithm
8. Formulate potential algorithm, and evaluate

Bare in mind that there is no good algorithm for creating algorithms, it's mainly a creative and trial and error process.

## Sorting Algorithms

#### Problem specification

`Input: array A[1...n]`

#### Required output

* A sorted
* Constraint: Sorting to be in situ (in position)

#### Layman Terms

Scan through the Array A, and compare each element within the array index n, swapping the values at the indexes based on whether their size is larger than the previous item at the previous index in the array.

### **Selection Sort** Pseudocode

![](<../../../../.gitbook/assets/image (195) (1) (1).png>)

### Bubble Sort Pseudocode

![](<../../../../.gitbook/assets/image (196) (1) (1).png>)

## Searching Algorithms

#### Problem specification

`Input: array A[1...n] and item M.`

#### Required output

* true – if M occurs in A.
* false – if M does not occur in A.

#### Layman Terms

Scan through the Array A, and compare each element at the array index n, with M.

### Sequential Search Pseudocode

![](<../../../../.gitbook/assets/image (194) (1) (1) (1).png>)
