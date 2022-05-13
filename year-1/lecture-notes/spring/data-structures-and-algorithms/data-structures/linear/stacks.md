# Stacks

A stack is an **abstract data type** that's a linear data structure. **Stacks use Last In First Out (LIFO)** to manage data.

* Use Push() and Pop() functions to add and remove elements from the stack. With push() adding onto the top of the stack, and pop() removing from the top of the stack.
* _Can be either Array based or List based._
* Not thought of as indexes
* Best way to think of it would be like washing up a tower of dirty dishes. It's best to remove from the top and work your way down.
* All insertions, removals and access is limited to the last element in the stack (top of the stack).

Applications Include

* Web browsers, they store recent web addresses onto a stack.
* Text editors with their undo option is stored on a stack (edit history).
* Calculators store operands and results on a stack.
* Runtime Memory Environments use a call stack to hold information about procedure calling.

If a stack is array-based, we must be aware of stack underflow (pop) and stack over-flow (push). Which means that creating stacks is more effecient with singly-linked lists. However, array based stacks are very effecient and safe, if you exclude over and underflow.

## Simple Array-Based Stack Implementation&#x20;

## Implementing a Stack with a Singly Linked List
