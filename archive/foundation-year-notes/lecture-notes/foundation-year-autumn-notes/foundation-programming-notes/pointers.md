# Pointers

## Pointers

To understand arrays, we must first understand pointers and [variables](variables-and-data-types.md#variables), as variables have pointers to their actual value, and arrays are a collection of variables (of the same data type). So one array maps to lots of elements, with an array pointer, and pointers to elements within the array. Also, _one way_ to pass arrays to functions you can pass to the function a **pointer **to an array by specifying the array's name without an index (so no square brackets)

A **pointer** is a variable whose value is the address of another variable, i.e. direct address of the memory location. Like any variable or constant, you must declare a pointer before using it to store any variable address. These are different to normal variables, as they store values of a specific data type. 

The general form of a pointer variable declaration is − `type *var-name;` There are more ways to denote a pointer:

* Pointer assigned to an address of a variable
  * `ptr = &var;`
* Dereferenced pointer, so 3 is added to var
  * `*ptr += 3;`

**Faster** and more efficient code USED TO BE written with pointers, as **pointers** are closer to the hardware. Now a days there isn't much of a performance difference, as **compilers are very optimized now a days,** compared to the earlier days. If you declare a variable as a register variable the compiler will do its utmost to ensure that it is stored in a register on the CPU. Accessing registers is much faster than accessing RAM, as variables are stored in the RAM. But now a days, compilers match the effeciency.

Pointers are the reason C is super fast. But also the reason why C is hard to manage. Pointers know the data type of the variable that they belong to.

De referencing a pointer means going to an address of a pointer.

As pointers directly change memory addresses, one function can essentially return multiple values, if the variables are passed by referenced and changes are made to the variables within the function.

The size of a pointer is defaulted to 4 bytes in 32-bit. And 8 bytes in 64-bit.

[Examples are on the code base.](https://adnantech.gitbook.io/code/code/c/pointers)
