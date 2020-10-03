# Types and Range of Programming Languages

### Types of Programming Languages

Types of programming languages can be referred to as **paradigms**. These paradigms can be further broken down:



* **Imperative** languages in which you instruct the computer _how_ to do a task, and 
* **Declarative** languages in which you tell the computer _what_ to do.

Range and Type of Programming Languages:

Machine \(binary\) code instructions consist of 1 and 0s and is used to communicate with hardware. Because it was so hard to write, assembly code was invented, where mnemonics were added. Converting assembly code to machine code is a one to one ratio.

 **Machine code** instructions are made up of:

* **Opcode** - A Single specific **numeric** instruction \(0001, 1000, 0101, 1000\)
* **Operand** - The **numeric** address of an element in the memory \(0000 0000 0011, 0000 0000 1101, 0000 0000 0110, 0000 0000 1101\)

**Assembly code** uses the same approach of Opcodes and Operatoes, in a more legible approach:

*  **Opcode** - A Single instruction displayed as a mnemonic \(ADD, LOAD, STORE, BRANCH, INPUT\)
*  **Operand** - The address of an element as an integer, with an addressing type: 
  * **xx - Direct Addressing** - The operand holds the **physical memory location** of the element to be operated on 
  * **&xx - Immediate Addresssing** - The operand contains the **value** of the element to be operated on 
  * **\#xx - Indirect Addressing** - The operand contains the **address** of the location in the physical memory, this location contains the physical address of the location in the memory where the value is stored 
  * **xx\[\] - Indexed Addressing** - Indexed addressing is used in machines containing an index register. With this mode of addressing, values in the operand are **offset** by the value stored in the index register

Higher level programming languages usually have specific purposes, SQL is for databses, C\# for windows applications, PHP for web applications. High level languages are also compiled into low level machine code. Scripting languages, such as PHP and JavaScript use interpreters, where each line is compiled as being run. Java is compiled into byte code \(virtual assembly code\), and then interpreted by a JVM \(java virutal machine\). Compilers turn high level code into machine code

