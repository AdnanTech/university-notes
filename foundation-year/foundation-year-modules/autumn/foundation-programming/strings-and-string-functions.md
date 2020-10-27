# Strings and String Functions

## String

* C does **not** have a string data type
* C does have string literals
* A string literal is a group of chars enclosed in double quotes.
* A string can be stored in a char arraybut must be terminated with a NULL character, which can be represented with ‘\0’. The last character of a string is always null.
* The assignment operator, ‘=’, can only be used when an array is declared. So a string cannot be copied using the assignment operator, ‘=’, in the body of your code.
* Relational operators cannot be used with strings.
* To copy strings and to compare strings we will need to use special functions in the string.h header file.

### Example of string in memory

![](../../../../.gitbook/assets/image%20%2811%29.png)

### [Examples on Code Base](https://adnantech.gitbook.io/code/code/c/arrays)



## String Functions

String Functions can be used to handle strings, such as manipulating strings, counting them, taking string input and more. This is important because most programs will eventually need string manipulation, and C does not have string handling functions in its original state.

So we add the header file  C supports a large number of string handling functions in the header file`include <string.h>`, this header file contains macro definitions for string handling functions

### String manipulation functions

| Function | Usage |
| :--- | :--- |
| strlen\(\) | Computes string's length |
| strcpy\(\) | copies a string to another |
| strcat\(\) | concatenates two strings |
| strcmp\(\) | Compares two strings |
| strlwr\(\) | Converts string to  |

### Special string functions

These are included in the stdio.h header file, but have massive usage in string handling functions

| Function | Usage |
| :--- | :--- |
| gets\(\) | Read string from user |
| puts\(\) | Displays the string |

## Header Files vs Library Files

* HEADER FILE is that in which declaration of a function is written.By using header file we can access a particular function while
* LIBRARY FILE is that in which definition of a particular function is written. MATH.H is a HEADER FILE while MATH.LIB is library file.

  
Header Files : These are the files that are included at the top of any program. If we use any function inside a program, then the header file containing declaration or definition of that function ,has to be included.Like printf\(\) is defined in stdio.h.So, we must include it \(by \#include in order to use printf\(\).

Library Files: These are the files which the compiler uses in order to define the functions which have been used in the program and had been declared inside the header file.Like, printf\(\) has its complete definition ,like how it will work etc. in an I/O library! So, the compiler uses that library to get the machine code for printf.

