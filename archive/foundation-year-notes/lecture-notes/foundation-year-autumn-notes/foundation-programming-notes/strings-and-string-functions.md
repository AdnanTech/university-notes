# Strings and String Functions

## String

* C does **not** have a string data type
* C does have string literals
* A string literal is a group of chars enclosed in double quotes.
* [A string can be stored in a char array but must be terminated with a NULL character, which can be represented with ‘\0’. The last character of a string is always null](https://stackoverflow.com/questions/20161921/null-byte-and-arrays-in-c), but not in a normal array \(not an array of single characters/not with a NON string literal\)
* The assignment operator, ‘=’, can only be used when an array is declared. So a string cannot be copied using the assignment operator, ‘=’, in the body of your code.
* Relational operators cannot be used with strings.
* To copy strings and to compare strings we will need to use special functions in the string.h header file.

### Example of string in memory

![](../../../../../.gitbook/assets/image%20%2811%29.png)

### [Examples on Code Base](https://adnantech.gitbook.io/code/code/c/arrays)

## Strings

### gets\(\), fgets\(\), puts\(\), scanf\(\)

These are all standard functions that handle input of strings. These functions do not require any header files, aside stdio. 

You can also make your own function to input strings. I have examples on the code base.

**Normal** operators **do not** work with strings. The reason for this is because each character is stored in an array, thus meaning each has a different value. Normal operators take only 1 value either side. You can create your own function to check if two strings are equal, by checking every character in both of the arrays to each other, one by one. Example is on the code base.

## String functions

### strcpy\(\)

Using the header file **string.h**, we can add some pre built functions to manipulate strings. One example is **strcpy\(\)**, which deletes a character in a string, by replacing the character with the character infront, and contuining the process till all characters are shifted backwards by one, essentially deleting the character chosen to be deleted by method of replacement.

### itoa\(\)

The function scanf\(\) converts keyboard input strings into various formats using field specifiers eg %d.The functions atoi\(\), atoll\(\) and atof\(\) do something similar with strings stored in memory. Using the header file **stdlib.h**. Functions like **itoa\(\)** convert in the opposite direction as shown in the code base.

itoa\(\) can converts a number into a strong of a different digit base. Binary, to hexadecimal, to octal or to denary. itoa\(\) is also a good function to print the reverse of numbers. Examples on code base.

### strlen\(\)

Used in string.h, the function is used to count length of a string. Example in code base.

### strcmp\(\)

Also used in string.h, the function is used to compare 2 strings.

## Class Notes

* gets\(\) is no longer ANSI standard because there is no boundary check.
  * Therefore you can overflow and corrupt memory if your string is too long
* fgets\(\) uses file concepts. The keyboard is the input, and the screen is the output. fgets\(\) also guards against buffer overflow
* [String Input conversion](http://www.gnu.org/software/libc/manual/html_node/String-Input-Conversions.html) - essentially regex to normalise scanf input
* To check equality of strings, since we can't apply relational operators to whole strings. Instead, we check each caracter one by one, to validate if they are the same.
* scanf\("%10\[^\n\]\) is a string literal - the 10 - cannot be changed, thus the max number of characters the scanf can take and store is 9, as we need one character for the null terminator. In these cases, where the size is variable, we can use fgets instead
* itoa\(\) stands for int to ascii \(string\)

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
| fgets\(\) | Read string from user using file input output concept |
| puts\(\) | Displays the string |

## Header Files vs Library Files

* HEADER FILE is that in which declaration of a function is written.By using header file we can access a particular function while
* LIBRARY FILE is that in which definition of a particular function is written. MATH.H is a HEADER FILE while MATH.LIB is library file.

  
Header Files : These are the files that are included at the top of any program. If we use any function inside a program, then the header file containing declaration or definition of that function ,has to be included. Like printf\(\) is defined in stdio.h.So, we must include it \(by \#include in order to use printf\(\).

Library Files: These are the files which the compiler uses in order to define the functions which have been used in the program and had been declared inside the header file. Like, printf\(\) has its complete definition ,like how it will work etc. in an I/O library! So, the compiler uses that library to get the machine code for printf\(\).

