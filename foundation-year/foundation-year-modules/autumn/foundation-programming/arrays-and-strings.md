# Arrays and Strings

## Pointers

To understand arrays, we must first understand pointers and [variables](variables-and-data-types.md#variables), as variables have pointers to their actual value, and arrays are a collection of variables \(of the same data type\). So one array maps to lots of elements, with an array pointer, and pointers to elements within the array. Also, _one way_ to pass arrays to functions you can pass to the function a **pointer** to an array by specifying the array's name without an index \(so no square brackets\)

A **pointer** is a variable whose value is the address of another variable, i.e. direct address of the memory location. Like any variable or constant, you must declare a pointer before using it to store any variable address. These are different to normal variables, as they store values of a specific data type. 

The general form of a pointer variable declaration is − `type *var-name;` 

Examples can be found [here](https://adnantech.gitbook.io/code/code/c/pointers).

## Buffers

Buffers can be flushed with `setbuf(stdout, NULL);` .**C** uses a **buffer** to output or input variables. The **buffer** stores the variable that is supposed to be taken in \(input\) or sent out \(output\) of the program. A **buffer** needs to be cleared before the next input is taken in.

Buffers are important because if not emptied, the input and output of any variables read from a user can be incorrectly displayed or cause the program to crash if the data types don't correspond to the incorrect data type. It's essentially validation of input data.

"A buffer is a block of memory where things can be stored" - Richard

## Array

Arrays a kind of **data structure** that can store a **fixed-size** sequential **collection** of elements \(variables\) of the **same** \(primitive\) **data type**. ****All arrays consist of contiguous **memory locations**. The _lowest_ address corresponds to the **first** element and the _highest_ address to the **last** element.

The general form of an array declaration is  − `datatype arrayName[arraySize];` Note: you do not have to specif

Initializing an array example: `double balance[5] = {1000.0, 2.0, 3.4, 7.0, 50.0};`

Another example of initializing arrays:

![](../../../../.gitbook/assets/image%20%281%29.png)

* An array is a list of variables with a shared name and data type.
* Each variable in the list is indexed by an integer inside square brackets and starts at 0.
* The square brackets tell the compiler that we are dealing with an array.
* The name of an array is a constant pointer that contains the address of the first variable\(slot\) in the array and its data type.
* The assignment operator, ‘=’, can be used to initialize an array when it is declared. After that, the assignment operator can only be used with individual slots within the array.
* Relational operators can only be used with individual slots within arrays.
* To copy an array or to compare arrays you will need to use a loop to access all the slots individually

