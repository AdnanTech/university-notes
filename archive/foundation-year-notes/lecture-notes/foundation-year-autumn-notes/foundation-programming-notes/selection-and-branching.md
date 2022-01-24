# Selection and Branching

Selection and branching dictate whether code should be run, or skipped, or go to another function, based on their boolean condition.

## Selection

A **selection** is used to make decisions on code to execute, depending on information such as a boolean condition being true or false. These condition involve _operators_ such as **relational, conditional,** **logical** or sometimes **all of themSelection**: used for _decisions_, **branching** -- choosing between _2 or_ more _alternative paths_.

The types of selection statements include **`if` ** statements, **`switch` (case)** statements and **`?`** statements (conditional operator).  The normal `if` works on _statements_, while the ? conditional operator works on _expressions_.

### Relational Operators

| Relational Operator | Operation                 |
| ------------------- | ------------------------- |
| ==                  | Equal to                  |
| !=                  | Not equal to              |
| <                   | Less than                 |
| >                   | Greater than              |
| <=                  | Less than or equal to     |
| >=                  | Greather than or equal to |

### Logical Operators

| Logical Operator | Operation   |
| ---------------- | ----------- |
| \|\|             | Logical OR  |
| &&               | Logical AND |
| !                | Logical NOT |

### Conditional Operator

The ? conditional operator, which is referred to as the ternary operator, evaluates an **expression** and assigns a value, based on a boolean condition. It can be seen as a shorthand way of using an if statement to assign a variable.

`varToBeAssigned = (conditional expression) ? expressionOne : expressionTwo` So if expression one is false, the variable is assigned to expression two, some examples below:

{% tabs %}
{% tab title="? Example 1" %}
```c
if (num1 > num2)
{
	max = num1;
}
else {max = num2;
}

/* is equivalent to: */
max = (num1 > num2) ? num1 : num2;
```
{% endtab %}

{% tab title="? Example 2" %}
```c
if (a > b)
{
    c = 25;
}
else
{
    c = 45;
}

/* is equivalent to: */
(a > b) ? (c = 25) : (c = 45);
```
{% endtab %}
{% endtabs %}
