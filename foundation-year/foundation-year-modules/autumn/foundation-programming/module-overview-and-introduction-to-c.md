# Module Overview and Introduction To C

## NOTES FROM 28/9

 Went through the module information page on canvas

Assessments: 1. Week 5 - canvas online quiz - 20% 2. Week 8 - programming project - 30% 3. Week 11 - programming project - 50% Hand in files as pdf doc or word

Mark scheme is on canvas: Style Rules for c programming 500 word evaluatioe ansi c so its not cross platform

 We are using ANSI C, which is the basic form of C avalible cross platform, this limits us to CLI applications only

 Reading list is given

 Contact information is given on canvas for: Ramiz, Kingsley, and Richard

 Programming languages we are going to learn, in order: C -&gt; C++ -&gt; Java

 If on mac, the alternative to dev C++ is XCode

 Microsoft Studo doesnt use standard ANSI C, so it is not cross platform

 Notes on Dev C++:

 There is no way to declare strings, you have to declare an array of characters that contain the string: char c\[\] = "c string";

 Compiler options

 ISOC99 is the default language for C we are using

 Show most warnings yes

 Editor options

 72 max width for a line

 4 spaces as tabs

 General c notes /\* is a comment

 Multiline comment at the start of the program /\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*

*  Program name
*  what the program does
*  author \(Adnan Quisar\)
*  version number/date

 \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*/

 You must start with include stdio.h And an int main that has void in parenthesis Curly brackets must have their own line





## NOTES FROM 29/9

 We a GNU Compiler for c code

 Dev C++ is a portable ide

 A non ide approach is to use clang on the mac

 You cant comment with //, has to be /\*

 "" is for string literal ' is for a single character

 You have to state void function\_name\(void\), you have to state this when writing functions that donnny data types

 Return 0 means no error code, even if you dons in, it is returned by default Include stdio.h is also implicity added even if it is not added in the top

 C has a lot of undefined behaviour as it is low level, so you mess around with memory locations



## NOTES FROM 30/9

 Range and Type of Programming Languages:

 Machine \(binary\) code instructions consist of 1 and 0s and is used to communicate with hardware. Because it was so hard to write, assembly code was invented, where mnemonics were added. Converting assembly code to machine code is a one to one ratio.

 Machine code instructions are made up of:

*  Opcode - A Single specific **numeric** instruction \(0001, 1000, 0101, 1000\)
*  Operand - The **numeric** address of an element in the memory \(0000 0000 0011, 0000 0000 1101, 0000 0000 0110, 0000 0000 1101\)

 Whereas Assembly code uses the same approach of Opcodes and Operatoes, in a more legible approach:

*  Opcode - A Single instruction displayed as a mnemonic \(ADD, LOAD, STORE, BRANCH, INPUT\)
*  Operand - The address of an element as an integer, with an addressing type: xx - Direct Addressing - The operand holds the **physical memory location** of the element to be operated on &xx - Immediate Addresssing - The operand contains the **value** of the element to be operated on \#xx - Indirect Addressing - The operand contains the address of the location in the physical memory, this location contains the physical address of the location in the memory where the value is stored xx\[\] - Indexed Addressing - Indexed addressing is used in machines containing an index register. With this mode of addressing, values in the operand are offset by the value stored in the index register

 Higher level programming languages usually have specific purposes, SQL is for databses, C\# for windows applications, PHP for web applications. High level languages are also compiled into low level machine code. Scripting languages, such as PHP and JavaScript use interpreters, where each line is compiled as being run.

 Java is compiled into byte code \(virtual assembly code\), and then interpreted by a JVM \(java virutal machine\)

 Compilers turn high level code into machine code

 C is compiled, compilation has some main stages: Lexical analysis, syntax analysis, code generation and code optimization. The end result an executable file of machine code.

*  Preprocessor uses a macro language to transform C code before compilation, for example adding in code from header files.
*  Linkers combines binary files together along with operating system static library files so they can be used in tandem to form an executable file. A good example of this is how Windows links all the .dll libraries together.

 There are different file states during C compilation:

*  Source Code \(.c\)
*  Substitutions \(.i\)
*  Assembly Code \(.s\)
*  Object \(machine\) Code \(.o\)
*  Executable \(.exe\)

 Only source files \(.c\), object code files \(.o\), and executable \(.exe\) are saved after compilation. To keep all files, change the compiler option **-save-temps**

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

 Lecture Notes:

*  if you include string.h at the sart, the functions to concatenate strins and len of strings
*  all variables have to be **camel case**, this is set to FILENAMES as well
*  Only use /\* for opening comments, and \*/ for closing comments
*  malloc can allocate dynamic memory to an element
*  fortan and cobol are old, dead programming languages
*  C is not an OOP language, we use structs and function pointers instead
*  exe is technically not machine code, as it is just instructions to the operating system, as the OS is a c program essentially
*  dont use underscores when naming variables
*  Ansi standard is to declare variables at the start of a code block \(functions, before branch statements\)

