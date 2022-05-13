# Arrays

Arrays are the simplest data structure.&#x20;

* They are fixed size and stored in the order they are inserted at via indexes.
* The first index is always zero.
* The memory allocation is static (sequentially in memory like blocks)
* Arrays can be as many dimensions as you want, with applications in matrixes, data storage and pretty much everywhere.

## Strengths

* Storing as many items as you can up to a known amount (inventory, stock)
* Finding items by index is very fast (4th element or 1st element etc)

## Weaknesses

* Removing elements at indexes, as you have to move all elements past the removed index up by 1, which can cost resources (average length of array / 2)
* Inserting into an ordered array means you need to inspect each element until you find the correct index to place the new element at.
