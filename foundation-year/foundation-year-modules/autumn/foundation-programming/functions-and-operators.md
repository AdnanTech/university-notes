# Functions and Operators

### Functions

* In **programming** a function \(method in OOP, procedure/subroutine if nothing is returned\) a block of code, which **given a set of any amount of parameters**, performs a task and can **return exactly one value**. Every C program has at least one function, which is main\(\), the main\(\) function is run on program execution, main\(\) in turn calls \(runs\) standard library functions and also user defined functions.
* In **maths** a function is an equation for which any given x into the equation, it will return exactly one y
* A **function prototype** \(declaration\) tells the compiler about a _function's name, return type, and parameters_. A function definition provides the actual body of the function
* printf\(\) and scanf\(\) are functions that are taken from the header file library
* You can define how many columns can be displayed to the console using a numeric precessor;
  * `printf("%2d", var)`- here var is displayed in a column that is 2 wide
* in C, there is a difference between num++ and ++num
  * `++i` will increment the value of `i`, and then return the incremented value.
  *  `i++` will increment the value of `i`, but return the original value that `i` held before being incremented.
* The **sizeof**\(\) **function** in C is a built-in **function** that is used to calculate the **size** \(in bytes\)that a data type occupies in ​the computer's memory
* **Refer to** [**Code Base** ](https://adnantech.gitbook.io/code/)**for C Function Examples**

### Operators

An **operator** is a symbol that tells the compiler or interpreter to perform specific mathematical, relational or logical operation and produce final result, the main types are arithmetic, assignment and relational.

{% hint style="info" %}
**Operators follow the order of precedence \(BEDMAS\)**
{% endhint %}

### There are 3 main types of operators

#### Arithmetic Operators

* An **operator is like a function**, where things get worked out and a value is returned. For example, with x + y the addition operator causes the value of x plus y to be returned. For an operator to work, it requires one or more OPERAND. So in the previous example, x and y are both operands. They would be called parameters for a function. Without one or the other, the addition operator won't work.

| Arithmetic operator | Operation |
| :--- | :--- |
| + | Addition |
| - | Subtraction |
| \* | Multiplacation |
| / | Division |
| % \(%% as a string\) | Modulus \(remainder of division\) |
| ++ \(var++ _for c_ or ++var for _c++_\) | Increment |
| -- \(- -\) | Decrement |

_Note on increment/decrement operator: if you assign a new variable, to the original variable, the order of precedence is **left to right**, for example:_

{% tabs %}
{% tab title="Incrementing and Decrementing when assigning variables" %}
```c
#include <stdio.h>

void TestingOne(void);
void TestingTwo(void);

int main(void)
{
    TestingOne();
    printf("\n");
    TestingTwo();
    return 0;                    
}

void TestingOne(void)
{
    int x = 5;
    int b;
    
    b = x++;
    printf("%d", b); /* 5 */
    printf("%d", x); /* 6 */
}

void TestingTwo(void)
{
    int x = 5;
    int b;
    
    b = ++x;
    printf("%d", b); /* 6 */
    printf("%d", x); /* 6 */
}
```
{% endtab %}
{% endtabs %}



#### Arithmetic assignment Operators

| Arithmetic Assignment Operator | Less efficient equivalent |
| :--- | :--- |
| x += y; | x = x + y; |
| x -= y; | x = x - y; |
| x \*= y; | x = x \* y; |
| x /= y; | x = x / y; |
| x %= y; | x = x % y; |

#### Relational Operators

| Relational Operator | Operation |
| :--- | :--- |
| &lt; | Less than |
| &gt; | Greater than |
| &lt;= | Less than or equal to |
| == | Equal to |
| != | Not equal to |

