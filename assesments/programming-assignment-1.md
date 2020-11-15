# Programming Assignment 1

{% file src="../.gitbook/assets/progproj1.pdf" caption="Project Brief" %}

{% file src="../.gitbook/assets/stylerulesc.pdf" caption="Style Rules" %}

## Planning

There can be a total of 15 matches \(8 first round, 4 quarter finals, 2 semi finals, 1 finals\), this means there can be 15 match results. You cannot draw in table tennis, simply put, it is get to 11 or get to 11 and win by 2.

### Structure

* We store the players in a 2d array
* we have a structure of the tournament called tournament round
* declare 4 round structures that contain
  * round one players
    * round one results
  * round quarter players
    * round quarter results
* etc



### Program Design

1. We start with prompting the user with 16 users
   1. For loop from 0 to 15, creating a new player struct after entered
2. Then go to the menu
   1. Enter a match result
      1. Ask user for a match number to enter results for
      2. Present board with input options \(print grid idea\)
   2. Display a round
      1. print grid idea \* round number
   3. Exit the program
      1. if user enters exit, exit

### Structures

**Need to send pointers**, as currently the structures are being passed as values, and not references. This means that when the structure is referenced beyond the funciton it is passed to, it will have different values.

### Top Down Design

There are 4 main functions, with 2 of them being reusable

* **Initialize**
  * take 16 names, one by one as input, and enter them into the first round appropriately
* **Menu**
  * Switch case statement, takes input as char \(mr/dr/e\), check style rules for switch case statements
    * **Enter a match result**
      * x, y \(player 1 x, player 2 y\) enter 1w if player 1 won the round, enter 2w if player 2, y, won the round. _\(conversely, you have the option to enter 1L if player 1 lost the round, this assumes player 2 has won the round\)_
    * **Display a round**
      * refer to bleow for design
    * **Exit the program**

### The grid \(Display a round\)

```c
************************************************************************
Match [matchnumber]
[Player 1]                W    L    W    W            
[Player 2]                L    W    L    L

Winner: [Player 1]
************************************************************************
```

### Research

* [Random old logic example](https://cboard.cprogramming.com/cplusplus-programming/108295-table-tennis-scoring-system.html)
* [Tournament bracket logic](https://stackoverflow.com/questions/6071563/algorithms-for-tournament-brackets-ncaa-etc)
* [scanf the effecient way](https://stackoverflow.com/questions/30065675/what-does-scanf-nc-mean)

{% file src="../.gitbook/assets/ip14\_advanced-4slides.pdf" caption="Reading Paper" %}

