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

that come with format specifiers, that are also stored in memory differently:

* **%c - char** - a single character 'A' \(notice the single quotes for a char\)
* **%d/%i - int** - an integer value 5
* **%f - float** - A floating-point number to 7 significant places 0.123456
* **%e - double** - a floating-point number to 15 significant places 0.1234567891234
* **%s - `char string_name[] (string)`** - string literal**s** "Hello World" \(notice the double quotes\)
* **%d - bool** - a boolean value 1 \(true\)

 Data types can also be modified:

*  int can be modified:
  *  long int
  *  short int
  *  long long int
  *  unsigned int
*  double can be modified:
  *  long double

#### Simple C examples:

printf\("hello world"\) - prints to console   
scanf\("Enter a value", &variableName\) - takes input from user

