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
{% tab title="2. Design Structure & Logic" %}
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

{% tabs %}
{% tab title="3. Creating Prototype Functions" %}
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
{% endtab %}
{% endtabs %}

### Creating Functions

Lastly, we tackle the functions in chroniclogical order, and compile and test the program

{% tabs %}
{% tab title="4. Creating Functions" %}
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
{% endtab %}
{% endtabs %}

## Iteration

Iteration is repitition until a condition is met, or forever.

### ASCII

Printing out UNICODE symbols \(must be run on UNICODE layout, not ASCII\), in hexademical form \(base 16\). Seperated by a tab. Note that the ASCII codes early on are empty because they cant be directly represented by a character \(NULL, Backspace, End, Shift, Return, Escape etc

{% tabs %}
{% tab title="Code" %}
```csharp
int main(void)
{
    int code;
    for(code = 1; code < 256; code++) /* codes 1 to 255 */
    {
        printf("%3x = %c\t", code, code); /* print code & character */
    }
    return 0;
}
```
{% endtab %}

{% tab title="Output" %}
      1 =    2 =    3 =    4 =    5 =    6 =    7 =     8 =     9 =             a =
              e =    f =   10 =   11 =   12 =   13 =   14 =   15 =   16 =   17 =   18 =   19 =   1a =   1b = 
             1c =   1d =   1e =   1f =   20 =    21 = !  22 = "  23 = #  24 = $  25 = %  26 = &  27 = '  28 = (  29 = )
             2a = *  2b = +  2c = ,  2d = -  2e = .  2f = /  30 = 0  31 = 1  32 = 2  33 = 3  34 = 4  35 = 5  36 = 6  37 = 7
             38 = 8  39 = 9  3a = :  3b = ;  3c = <  3d = =  3e = >  3f = ?  40 = @  41 = A  42 = B  43 = C  44 = D  45 = E
             46 = F  47 = G  48 = H  49 = I  4a = J  4b = K  4c = L  4d = M  4e = N  4f = O  50 = P  51 = Q  52 = R  53 = S
             54 = T  55 = U  56 = V  57 = W  58 = X  59 = Y  5a = Z  5b = [  5c = \  5d = ]  5e = ^  5f = _  60 = `  61 = a
             62 = b  63 = c  64 = d  65 = e  66 = f  67 = g  68 = h  69 = i  6a = j  6b = k  6c = l  6d = m  6e = n  6f = o
             70 = p  71 = q  72 = r  73 = s  74 = t  75 = u  76 = v  77 = w  78 = x  79 = y  7a = z  7b = {  7c = |  7d = }
             7e = ~  7f =   80 = Ç  81 = ü  82 = é  83 = â  84 = ä  85 = à  86 = å  87 = ç  88 = ê  89 = ë  8a = è  8b = ï
             8c = î  8d = ì  8e = Ä  8f = Å  90 = É  91 = æ  92 = Æ  93 = ô  94 = ö  95 = ò  96 = û  97 = ù  98 = ÿ  99 = Ö
             9a = Ü  9b = ø  9c = £  9d = Ø  9e = ×  9f = ƒ  a0 = á  a1 = í  a2 = ó  a3 = ú  a4 = ñ  a5 = Ñ  a6 = ª  a7 = º
             a8 = ¿  a9 = ®  aa = ¬  ab = ½  ac = ¼  ad = ¡  ae = «  af = »  b0 = ░  b1 = ▒  b2 = ▓  b3 = │  b4 = ┤  b5 = Á
             b6 = Â  b7 = À  b8 = ©  b9 = ╣  ba = ║  bb = ╗  bc = ╝  bd = ¢  be = ¥  bf = ┐  c0 = └  c1 = ┴  c2 = ┬  c3 = ├
             c4 = ─  c5 = ┼  c6 = ã  c7 = Ã  c8 = ╚  c9 = ╔  ca = ╩  cb = ╦  cc = ╠  cd = ═  ce = ╬  cf = ¤  d0 = ð  d1 = Ð
             d2 = Ê  d3 = Ë  d4 = È  d5 = ı  d6 = Í  d7 = Î  d8 = Ï  d9 = ┘  da = ┌  db = █  dc = ▄  dd = ¦  de = Ì  df = ▀
             e0 = Ó  e1 = ß  e2 = Ô  e3 = Ò  e4 = õ  e5 = Õ  e6 = µ  e7 = þ  e8 = Þ  e9 = Ú  ea = Û  eb = Ù  ec = ý  ed = Ý
             ee = ¯  ef = ´  f0 = ­  f1 = ±  f2 = ‗  f3 = ¾  f4 = ¶  f5 = §  f6 = ÷  f7 = ¸  f8 = °  f9 = ¨  fa = ·  fb = ¹
             fc = ³  fd = ²  fe = ■  ff =
{% endtab %}
{% endtabs %}

### Tables

Refer to [**Code base**](https://adnantech.gitbook.io/code/code/c/iteration) for Iteration examples

A small block of code to print out the times table up to 12.

{% tabs %}
{% tab title="Code" %}
```csharp
#include <stdio.h>
int main(void)
{
    int col, row;
    for(row = 1; row < 13; row++) /* for each row */
    {
        for(col = 1; col < 13; col++) /* for each column */
        {
            printf("%4d", col * row); /* print result */
        }
        printf("\n"); /* new line */
    }
    return 0;
}
```
{% endtab %}

{% tab title="Output" %}
```
   1   2   3   4   5   6   7   8   9  10  11  12
   2   4   6   8  10  12  14  16  18  20  22  24
   3   6   9  12  15  18  21  24  27  30  33  36
   4   8  12  16  20  24  28  32  36  40  44  48
   5  10  15  20  25  30  35  40  45  50  55  60
   6  12  18  24  30  36  42  48  54  60  66  72
   7  14  21  28  35  42  49  56  63  70  77  84
   8  16  24  32  40  48  56  64  72  80  88  96
   9  18  27  36  45  54  63  72  81  90  99 108
  10  20  30  40  50  60  70  80  90 100 110 120
  11  22  33  44  55  66  77  88  99 110 121 132
  12  24  36  48  60  72  84  96 108 120 132 144
```
{% endtab %}
{% endtabs %}

