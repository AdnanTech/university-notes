# Queues

A queue is an **abstract data type** that's a linear data structure, a restricted list structure. **Queues use First In First Out (LIFO)** to manage data. These can be array based or singly list based like stacks. The variants of Queues include the circular queue and the double-ended queue (deque, pronounced deck). Queues can thought of as linear in-out structures.

**Important Characteristics include:**

* All insertion takes place at the back, and is removed at the front
* There is a wrap around policy for Arrays
* enqueue(e) is at the front, dequeue() refers to the rear.
* **Queues do not have to have a specific capacity**
* _**Just like Stacks, we have an inherent problem where the worst case could be O(n) if you happen to run out of space on that particular add.**_

There is a **wrap around policy for arrays**. This negates the naivety of considering the end of memory as the max amount of possible items:

![](<../../../../.gitbook/assets/image (205).png>)

Abstract Data Types are defined by interfaces in Java. Meaning to code a Queue you need to define the interface.

**Applications of queues include:**

* Access for shared resources
  * Queue of jobs for a printer
  * **Scheduling CPU access in a multitasking OS (priority queue)**
  * Serving web-site requests
* **Shortest Path Algorithms, sorting collections (priority queue)**
* Asynchronous data transfer between processes
  * I/O buffering
  * Pipes and Sockets
* Playlist buffers
* Simulation of real workd queuing

## Queues / The Queue Abstract Data Type

![](<../../../../.gitbook/assets/image (200) (1).png>)

## Array-Based Queue Implementation

## Implementing a Queue with a Singly Linked List

## Circular Queue

Amazing for turn-based games and scheduling.&#x20;

Advantages include that you only need one pointer (tail) and you can traverse all list elements starting at any place.

To implement it, it would look like a circular linked list, except you only need a tail.

![](<../../../../.gitbook/assets/image (206).png>)

## Double-Ended Queues (Deque, Dequeue)

Double ended queues add the functionality of insertion at both the front and the rear of the queue.

Application example: Occasionally, the first person might be removed from the queue only to find that a table was not available; typically, the restaurant will reinsert the person at the first position in the queue. It may also be that a customer at the end of the queue may grow impatient and leave the restaurant.

Can be implemented using either arrays or linked lists. Array based implementation is a circular array, expanding storate when needed. A linked list implementation involves copying a doubly linked list and adding functionality.

## Implementing a Deque

## The Priority Queue Abstract Data Type

A priority queue is a collection of prioritised elements. They support element insertion and removal in order of priority.

The contrast here is that storage/acess are based on priority instead of linear position. This is what sets them apart to arrays, linked lists, stacks and other queues.

Applications include sorting algorithms (insertion, bubble and heap), shortest path algortihms (routing, networks) and scheduling/resource management of the CPU.

A priority queue can be defined as a collection with **keys and values (Key-Value pairs)**. The keys have to be comparable objects, as they define the priority. So adding and removal of elements is based on priority, and insertion adds entry with the given priority to queue. _Example of keys include lexicographic order on strings, age, time spent waiting etc_

Priority queues can be implemented using Arrays, Linked lists and heaps. Array and Linked list priority queues can be sorted or non-sorted.

Comparison in a priority queue (incase 2 things have the same key):

![](<../../../../.gitbook/assets/image (207).png>)

A relation having the connex property means that any pair of elements in the set of the relation are comparable under the relation.Implementing a Priority Queue. For this reason, when we implement priority queues in Java we need to take into consideration to add a 'comparable' interface.

Time complexity of priority queues can vary:

![](<../../../../.gitbook/assets/image (199).png>)

## Implementing a Priority Queue with an Unsorted List

## Implementing a Priority Queue with a Sorted List
