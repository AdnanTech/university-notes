# Program Design and Iteration

## Program Design

In this lecture we will cover writing a times table program which requests a table number and then displays the appropriate table

### Screen Design

First we design the screen, what we want the end result to look like

* This gives the dialogue between the user and computer. It also gives the order of the actions required

{% tabs %}
{% tab title="1. Screen Design" %}
```text
Times Table
===========

Enter table numner: !!

1 X !! = ???
2 X !! = ???
3 X !! = ???
4 X !! = ???
5 X !! = ???
6 X !! = ???
7 X !! = ???
8 X !! = ???
9 X !! = ???
10 X !! = ???
11 X !! = ???
12 X !! = ???

Hit any character to continue
```
{% endtab %}
{% endtabs %}

### Design the Structure and Logic of the Code

Secondly, we desing the structure and logic of the code

* This means using stepwise refinement \(top-down design\) to produce the program skeleton
* Starting with the main\(\) function and slowly building the program skeleton
  * Until the final program is achieved
* We use the screen design to work out the order of the actions involved in the program. We put a comment in main\(\) for each task identified. Compile and test the program.

{% tabs %}
{% tab title="Design Structure & Logic" %}
```csharp
/***********************************************************************
* timesTable.c
* Writing a times table program which requests a table number and then
* displays the appropriate table.
* Adnan Quisar
* October 2020
* ********************************************************************/

#include <stdio.h>
/* Function prototypes */
int main(void)
{
 /* Display title */
 /* Get the table number from the keyboard */
 /* Loop to display 12 lines of the table */
 /* Pause and wait for the enter key */
 return 0;
}
```
{% endtab %}
{% endtabs %}

### Creating Prototype Functions

Thirdly. we design protoype functions, these meet the following criteria

* Create the name for each function and check that the correct data type can be passed between the functions as required.
* Create the prototypes for each function and create the skeleton definition of each function.
* Add a comment to summarize each function above it
* In this example the displayTitle\(\) is entered first as it is an easy display function
* Compile and test the program.

```csharp
/***********************************************************************
* timesTable.c
* Writing a times table program which requests a table number and then
* displays the appropriate table.
* Adnan Quisar
* October 2020
* ********************************************************************/

#include <stdio.h>

/* Function prototypes */
void displayTitle(void);
int getTableNum(void);
void displayTable(int table);
void pause(void);

int main(void)
{
    int tableNo;
    /* Display title */
    displayTitle();
    /* Get the table number from the keyboard */
    tableNo = getTableNum();
    /* Loop to display 12 lines of the table */
    displayTable(tableNo);
    /* Pause and wait for the enter key */
    pause();
    return 0;
}

/* Display title */
void displayTitle(void)
{
    printf("Times Table\n");
    printf("===========\n\n");
}

/* Get the table number from the keyboard */
int getTableNum(void)
{
    return 7;
}

/* Loop to display 12 lines of the table */
void displayTable(int table)
{
    printf("Times Table %d\n", table);
}

/* Pause and wait for the enter key */
void pause(void)
{
}
```

### Creating Functions

Lastly, we tackle the functions in chroniclogical order, and compile and test the program

```csharp
/***********************************************************************
* timesTable.c
* Writing a times table program which requests a table number and then
* displays the appropriate table.
* Adnan Quisar
* October 2020
* ********************************************************************/

#include <stdio.h>

void displayTitle(void);
int getTableNum(void);
void displayTable(int table);
void pause(void);
void emptyBuffer(void);

int main(void)
{
    int tableNo;
    displayTitle();
    tableNo = getTableNum();
    displayTable(tableNo);
    pause();
    return 0;
}

/* Display title */
void displayTitle(void)
{
    printf("Times Table\n");
    printf("===========\n\n");
}

/* Get the table number from the keyboard */
int getTableNum(void)
{
    int table;
    printf("Enter table number: ");
    scanf("%d", &table);
    getchar();
    return table;
}

/* Loop to display 12 lines of the table */
void displayTable(int table)
{
    int line;
    for(line = 1; line <= 12; line++)
    {
        printf("%2d x %d = %3d\n", line, table, table * line);
    }
    printf("\n");
}

/* Pause and wait for the enter key */
void pause(void)
{
printf("\nPress the Enter key to continue.\n");
getchar();
}
```

## Iteration

