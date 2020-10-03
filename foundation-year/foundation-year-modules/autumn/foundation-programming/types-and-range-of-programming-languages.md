# Types and Range of Programming Languages

### Types of Programming Languages

Short version is High level, which is compiled into assembly code, which is then turned into machine code to be executed, and low level which is also compiled, but has to do less compiling as the programming langues like C are already assmebly code with syntatic sugar.

Long version is that the types of **programming languages** go under the class of **programming** **paradigms**. These paradigms can be further broken down, here i will cover 2 significant paradigms:

* **Imperative**: in which you instruct the computer _how_ to do a task
  * **Procedural**: in which a program is constructed by composing subroutines \(functions\), these subroutines contain a series of computational steps to be carried out, at any time when called during program execution.
    * Examples include: C and Pascal, and in older times FORTRAN and COBOL.
  * **Object Oriented**: in which a program is contructed by "_objects_", which contain data and code. _**Data**_ in the form form of _fields_ \(attributes and properties\), and _**code**_ in the form of _procedures_ \(methods\)
    * Examples include: C++, Java, C\#, VB.NET, PHP
* **Declarative**: in which you tell the computer _what_ to do
  * **Functional**: in which a program is constructed by applying \(passing arguments\) and composing \(combining\) functions. _Functions_ can be defined as **trees of expressions** \(entities: variables, constants, operators\) that can compound to each return a \(new\) value.
    * Examples include: Common Lisp, Wolfram Language [\(used to calculate the variables of the simulation of our universe!\)](https://www.youtube.com/watch?v=-t1_ffaFXao), Erlang, Haskell, Scheme
  * **Logic**: in which a program is constructed by a set of sentences in logical form that express facts and rules about a problem domain
    * Examples include: Prolog, Answer Set Programming \(ASP\), Datalog
  * **Constraint**: in which a program is constructed by declaratively stating the constraints on a solution for a set of decision variables
    * Examples include: Prolog III, CHIP, CLP\(R\)
  * **Data flow**: 

{% hint style="info" %}
The difference between functional and procedural is that functional takes arguments and returns a value, whereas procedural is simply a sequence of computational sequential steps
{% endhint %}

### Range of Programming languages

High level

* python adn MATLAB are multi paradigm

Low level

### Machine and Assmebly Code

All code is eventually turned into machine code. Assembly code is the more legible format of machine code. Machine \(binary\) code instructions consist of 1 and 0s and is used to communicate with hardware. Because it was so hard to write, assembly code was invented, where mnemonics were added. Converting assembly code to machine code is a one to one ratio.

 **Machine code** instructions are made up of:

* **Opcode** - A Single specific **numeric** instruction \(0001, 1000, 0101, 1000\)
* **Operand** - The **numeric** address of an element in the memory \(0000 0000 0011, 0000 0000 1101, 0000 0000 0110, 0000 0000 1101\)

**Assembly code** uses the same approach of Opcodes and Operatoes, in a more legible approach:

*  **Opcode** - A Single instruction displayed as a **mnemonic** \(ADD, LOAD, STORE, BRANCH, INPUT\)
*  **Operand** - The address of an element as an **integer** \(12, 04, 50, 38\) with an addressing type: 
  * **xx - Direct Addressing** - The operand holds the **physical memory location** of the element to be operated on 
  * **&xx - Immediate Addresssing** - The operand contains the **value** of the element to be operated on 
  * **\#xx - Indirect Addressing** - The operand contains the **address** of the location in the physical memory, this location contains the physical address of the location in the memory where the value is stored 
  * **xx\[\] - Indexed Addressing** - Indexed addressing is used in machines containing an index register. With this mode of addressing, values in the operand are **offset** by the value stored in the index register

Higher level programming languages usually have specific purposes, SQL is for databses, C\# for windows applications, PHP for web applications. High level languages are also compiled into low level machine code. Scripting languages, such as PHP and JavaScript use interpreters, where each line is compiled as being run. Java is compiled into byte code \(virtual assembly code\), and then interpreted by a JVM \(java virutal machine\). Compilers turn high level code into machine code

### Sources

[https://en.wikipedia.org/wiki/Object-oriented\_programming](https://en.wikipedia.org/wiki/Object-oriented_programming)  
[https://www.typesnuses.com/types-of-programming-languages-with-differences/](https://www.typesnuses.com/types-of-programming-languages-with-differences/)

