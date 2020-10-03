# Variables and Data Types



---Variables

*  A variable is a container in which a data value is stored inside the physical memory
*  Variables can be called by their assigned name
*  Variables must start with a letter or underscore
*  Variables names can contain letters, numbers or underscores
*  Variable names cannot be C reserved words \(True, if\)
*  Variables must be declared at the start of a block of code
*  Declaration syntax: **data-type variable-name**

 Data types, that come with format specifiers, that are also stored in memory differently:

*  %c - Char - a single character 'A' \(notice the single quotes for a char\)
*  %d/%i - int - an integer value 5
*  %f - float - A floating-point number to 7 significant places 0.123456
*  %e - double - a floating-point number to 15 significant places 0.1234567891234
*  %s - char string\_name\[\] \(string\) - string literals "Hello World" \(notice the double quotes\)
*  %d - bool - a boolean value 1 \(true\)

 Data types can also be modified

*  int can be modified:
  *  long int
  *  short int
  *  long long int
  *  unsigned int
*  double can be modified:
  *  long double

 printf\("hello world"\) - prints to console scanf\("Enter a value", &variable\) - takes input from user

 General C notes:

*  Global variables can be decalred above the main function
*  Constants can also be decalred by saying const
*  void functions can be called via void function\_name\(parameters\)
*  \#include &lt;iostream&gt; std::cout &lt;&lt; someString &lt;&lt; "\n"; is a different way of printing - this doesnt work in c, only c++ also try cout &lt;&lt; str;
*  arrays must be defined in length, if you are storing them later on, or you can define the length if you define the array on the same line
*  asterixes are used \(\*\) to represent a pointer to a memory location, NOT the value

