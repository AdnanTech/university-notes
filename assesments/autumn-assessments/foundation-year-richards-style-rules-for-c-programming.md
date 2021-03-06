# Richard's Style Rules for C Programming

{% file src="../../.gitbook/assets/stylerulesc \(1\).pdf" caption="Richard\'s Style Rules For C PDF " %}

## IDE Options \(DEV-C++\)

* DEV-C++ is the IDE we use
  * [Desktop App Download Link](https://sourceforge.net/projects/orwelldevcpp/files/Setup%20Releases/)
  * [Portable USB Application Download Link](https://sourceforge.net/projects/orwelldevcpp/files/Portable%20Releases/)
* Compiler Options:
  * Go into Tools -&gt; Compiler options at the top
    * _Go into settings and under C Options, Support all ANSI Standard C Programs should be set to Yes \(?\)_
    * Under Code generation, Language Standard is ISO C99
    * Under Warnings, Show most warnings should be set to Yes
* Editor Options
  * Go into Tools -&gt; Editor options at the Top
    * Under Right Margin, the Enabled box should be checked, and the width should be set to 72
    * Under Tabs, Use tab character should be unchecked, and Tab Automatically indents should be checked, along with the default tab size being 4

## General C Notes

* /\* comment \*/ is the standard for comments, any other method will be penalised
* All variables have to be **camel case**, this is set to fileNames as well
* Ansi standard is to declare variables at the start of a code block \(functions, before branch statements\)
* Dont use underscores when naming variables. 
* You must start with include stdio.h And an int main that has void in parenthesis 
* Curly brackets must have their own line
* You have add void in the brackets for functions that do not return anything: void function\_name\(**void**\)
* count variables also must be declared before the block of code
* Do not use the typedef struct statement found in some books. Using it can lead to confusion when we do C++. My house style is to always use struct identifier.
* 5 +- 2 lines per function
* Programs must start with the following multiline comment
  * ```c
    /***********************************************************************
    * programName.c
    * What the CLI application does
    * Author (Adnan Quisar)
    * Version Number/Start Date

    ```

## Functions

* Function prototypes listed before main\(\)
* Function definitions after main\(\). 
* Every function definition should be preceded by a comment.

## Program Design

Refer to Program Design notes, as a guideline, 2-7 lines of code per function, but only as a guideline

* level 1 skeleton code

Arrays cannot be dynamic in ANSI standard. They can only be a fixed size. There must also be a space beside either side of the curly brackets.

Constants are to be in ALL UPPERCASE letters

