# Arrays and Buffers

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
* Arrays can also be 2d, this can be useful for storing things such as co-ordinates
* The variable name of the Array is a pointer itself, it cannot be changed once the array has been declare
* The pointer points to the first item in the array
* You can only copy items of an array to another array. You cannot copy a whole array.
* If you declare an array of one size, it is \[1\], even though it only has 1 item \(2 memory pieces\), this is so you have at least one pointer for the array, and then that can point to the array name and the first slot.
* The end of the array is only known at compile time
* 
