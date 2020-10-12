# Introduction To C, use of the IDE, C Compilation

## Introduction to C

* C is a low level language, its essentially assembly code with syntatic sugar \(caveat is essentially, there are differences\).
* **For code examples visit** [**my codebase**](https://adnantech.gitbook.io/code/code/c/)\*\*\*\*
* We are using ANSI C, which is the basic form of C avalible cross platform, this limits us to CLI applications only. Microsoft Studio doesnt use standard ANSI C, so it is not cross platform. 
* C is not an OOP language, it is procedural. We can use structs and function pointers to imitate OOP although they are not the same.
* we use a GCC Compiler built into dev C++ to compile c code. A non ide approach is to use clang and vim on the mac. 
* Return 0 on an int function means no error code, even if you dont put it in, it is assumed to be return 0 by default 
* `include stdio.h` is also implicity added even if it is not added in the top
* C has a lot of undefined behaviour as it is low level, so you mess around with memory locations.
* If you `include string.h` at the sart, the functions to concatenate strings and len of strings.
* Malloc can allocate dynamic memory to an element. f
* .exe files are technically not machine code, as it is just instructions to the operating system, as the OS is a c program essentially. The OS takes those instructions and executes them as machine code instructions

### Header files

Header files serve two purposes.

*  System header files declare the interfaces to parts of the operating system. You include them in your program to supply the definitions and declarations you need to invoke system calls and libraries.
* Your own header files contain declarations for interfaces between the source files of your program. Each time you have a group of related declarations and macro definitions all or most of which are needed in several different source files, it is a good idea to create a header file for them.

## Use of the IDE

The Integrated Development Environment \(IDE\) we use is called Dev C++, it is windows only, and is possible to be downloaded as a portable application. IDE's allow us to compile and run code and keep track of files easier, as they come with customisable integrated compilers, text editors, linkers and assemblers.

## Compilation

C is compiled, general compilation has some main stages: Lexical analysis, syntax analysis, code generation and code optimization. The end result an executable file of machine code, below is the C compilation process

* Preprocessor uses a macro language to transform C code before compilation, for example adding in code from header files.
* The compiler then translates the C code into assembly code
* The assembler converts assembly code into machine code to create a binary object code file
* Linkers combines binary files together along with operating system static library files so they can be used in tandem to form an executable file. A good example of this is how Windows links all the .dll libraries together.
  * In C, the linker combines library functions and previously compiled functions, NOT header and batch files, as the header files is compiled and included in the program before compilation. Header files are NOT libraries.  A header file is a file containing C declarations and macro definitions to be shared between several source files

There are different file states during C compilation:

* Source Code \(.c\)
* Substitutions \(.i\)
* Assembly Code \(.s\)
* Object \(machine\) Code \(.o\)
* Executable \(.exe\)

Only source files \(.c\), object code files \(.o\), and executable \(.exe\) are saved after compilation. To keep all files, change the compiler option **-save-temps**

