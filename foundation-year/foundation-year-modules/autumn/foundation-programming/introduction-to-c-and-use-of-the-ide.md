# Introduction To C, use of the IDE, C Compilation

### Introduction to C

We are using ANSI C, which is the basic form of C avalible cross platform, this limits us to CLI applications only, however it is cross platform. Microsoft Studo doesnt use standard ANSI C, so it is not cross platform. C is not an OOP language, we use structs and function pointers instead we use a GNU Compiler to compile c code. A non ide approach is to use clang and vim on the mac. Return 0 means no error code, even if you dont put it in, it is returned by default Include stdio.h is also implicity added even if it is not added in the top. You must start with include stdio.h And an int main that has void in parenthesis Curly brackets must have their own line. C has a lot of undefined behaviour as it is low level, so you mess around with memory locations. if you include string.h at the sart, the functions to concatenate strins and len of strings. malloc can allocate dynamic memory to an element. fortan and cobol are old, dead programming languages. exe is technically not machine code, as it is just instructions to the operating system, as the OS is a c program essentially. dont use underscores when naming variables. 

### Use of the IDE

The Integrated Development Environment \(IDE\) we use is called Dev C++, it is windows only, and is possible to be downloaded as a portable application. IDE's allow us to compile and run code and keep track of files easier.

### Compilation

C is compiled, compilation has some main stages: Lexical analysis, syntax analysis, code generation and code optimization. The end result an executable file of machine code.

* Preprocessor uses a macro language to transform C code before compilation, for example adding in code from header files.
* The compiler then translates the C code into assembly code
* The assembler converts assembly code into machine code to create a binary object code file
* Linkers combines binary files together along with operating system static library files so they can be used in tandem to form an executable file. A good example of this is how Windows links all the .dll libraries together.

There are different file states during C compilation:

* Source Code \(.c\)
* Substitutions \(.i\)
* Assembly Code \(.s\)
* Object \(machine\) Code \(.o\)
* Executable \(.exe\)

Only source files \(.c\), object code files \(.o\), and executable \(.exe\) are saved after compilation. To keep all files, change the compiler option **-save-temps**

