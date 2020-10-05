# Variables and Data Types

### Variables

*  A variable is a container in which a data value is stored inside the physical memory
*  Variables can be called by their assigned name
*  Variables must start with a letter or underscore
*  Variables names can contain letters, numbers or underscores
*  Variable names cannot be C reserved words \(True, if\)
*  Variables must be declared at the start of a block of code
*  Declaration syntax: **data-type variable-name**
* There is no way to declare strings, you have to declare an array of characters that contain the string: `char c[] = "c string";`

### Data types

There are lots of data types, below are some of the primitive data types. In C, data types come with format specifiers, which means that the types are also stored in memory differently:

| Data Type | Format \(field\) Specifier | Examples \(in C\) |
| :--- | :--- | :--- |
| char | %c | printf\("char var = %c", var\); |
| int | %d / %i | printf\("int var = %d", var\); |
| float | %f | printf\("float var = %f", var\); |
| double | %lf \(LF\) | printf\("double var = %lf", var\); |
| double \(engineer notation\) | %e | printf\("double var = %e", var\); |
| \(string\) literals | %s | printf\("string var = %s", var\); |
| bool | %d | printf\("bool var = %d\n", var\); |

* **%c - char** - a single character 'A' \(notice the single quotes for a char\)
* **%d/%i - int** - an integer value 5
* **%f - float** - A floating-point number to 7 significant places 0.123456
* **%e - double** - a floating-point number to 15 significant places 0.1234567891234
* **%s - `char string_name[] (string)`** - string literal**s** "Hello World" \(notice the double quotes\)
* **%d - bool** - a boolean value 1 \(true\)

 Data types can also be _**modified**_:

*  int can be modified:
  *  long int
  *  short int
  *  long long int
  *  unsigned int
  * signed int
*  double can be modified:
  *  long double

### [C code examples on my Codebase](https://adnantech.gitbook.io/code/code/c)

