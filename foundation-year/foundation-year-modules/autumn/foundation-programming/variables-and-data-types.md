# Variables and Data Types

## Variables

*  A variable is a container in which a data value is stored inside the physical memory
*  Variables can be called by their assigned name
*  Variables must start with a letter or underscore
*  Variables names can contain letters, numbers or underscores
*  Variable names cannot be C reserved words \(True, if\)
*  Variables must be declared at the start of a block of code
*  Declaration syntax: **data-type variable-name**
* There is no way to declare strings, you have to declare an array of characters that contain the string: `char c[] = "c string";`

## Data types

There are lots of data types, below are some of the primitive data types. In C, data types come with format specifiers, depending on the data type, will determine how the data is stored in malloc \(memory\) differently:

| Data Type | Format \(field\) Specifier | Examples \(in C\) |
| :--- | :--- | :--- |
| char | %c | `printf("char var = %c", var);` |
| signed int | %d / %i | `printf("int var = %d", var);` |
| unsigned int | %u | `printf("int var = %u", var);` |
| short int | %dh / %ih | `printf("int var = %dh", var);` |
| float | %f | `printf("float var = %f", var);` |
| long double | %lf \(LF\) / .1lf \(1 d.p\) | `printf("double var = %lf", var);` |
| double \(engineer notation\) | %e | `printf("double var = %e", var);` |
| \(string\) literals | %s | `printf("string var = %s", var);` |
| bool | %d | `printf("bool var = %d\n", var);` |

* **%c - char** - a single character 'A' \(notice the single quotes for a char\)
* **%d/%i - int** - an integer value 5
* **%f - float** - A floating-point number to 7 significant places 0.123456
  * Use an exponent and mantissa
* **%e - double** - a floating-point number to 15 significant places 0.1234567891234
* **%s - `char string_name[] = "Hello World"`** - string literal**s** "Hello World" \(notice the double quotes\)
* **%d - bool** - a boolean value 1 \(true\)

 Data types can also be _**modified**_:

*  int can be modified:
  *  long int
    * 4 bytes long \(32 bit, higher range\)
  *  short int
    * 2 bytes long \(16 bit, lower range\)
  * long long int
    * atleast 64bit
  * unsigned int
    * cannot be negative, higher range
  * signed int
    * can be negative, lower range
*  double can be modified:
  *  long double
    * 16 bytes \(128 bit\)

### [Code Base C examples](https://adnantech.gitbook.io/code/code/c)

