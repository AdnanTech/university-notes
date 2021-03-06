# Testing

The point of testing a program is to find as many bugs as possible. Once the testing has had its first pass, decisions are needed to decide the priority order of correcting each error. Time, resources and lack of knowledgemay not allowforall errors to be corrected. Withmost large applications a list of known bugs is maintained. 

Test plans normally start of by checking basic functionality with simple valid data. This is then followed by checking boundaries, special values, input data types, must enter fields, format of data etc.

## Test plan

Test plans come first, and they should look something like \(for the table tennis knockout assignment\):

| Test ID | Feature | Test cases \(Input data\) | Expected Result | Details |
| :---: | :--- | :--- | :--- | :--- |
| 1 | Entering the 16 player names | Adnan Quisar, Adnan, A very very very very long name, 12 | Adnan Quisar, Adnan, A very very very ver, 12 | Max name length is 21 characters, including the NULL terminator |
| 2 | Entering which of the 2 players won the games | 1, 2, 0, 6, a, abc | Pass, pass, Error message \(prompts user to try again\), Error message \(prompts user to try again\), Error message \(prompts user to try again\), Error message \(prompts user to try again\) | Error handling message will be in place to ensure user does not try to enter an invalid data type or an integer outside of the values 1 or 2 |

## Test Log

After the program is developed, the test log should be carried out, which looks something like this \(based on the assignment\):

| Test ID | Actual Result | Comments |
| :--- | :--- | :--- |
| 1 | Adnan Quisar, Adnan, A very very very ver, 12 | Size of array is 21 characters, the terminating character stores the ‘\0’ character, therefore we have a max length of 20 characters. This means the program does not allow for anyone whose desired player name is over 20 characters in length, as it will not fully display. This was the intended result as I assume for users to enter only their first name and perhaps an abbreviation is required. In addition, if they wish to enter a player number instead of a name, the option is there, due to the character array being able to store integer input as a string, as integers are a part of the ascii character set. |
| 2 | Pass, pass, handled error, handled error, handled error, handled error, | Since 1 and 2 are the only valid score options, and it is easy to mess it up, I decided to add fully fledged validation checks to the score input of the match currently being played. This means, any character/s other than 1 or 2, for example 0, 6, a, abc and anything else, all display an error message, and no player score is incremented. I am extremely pleased with how this feature turned out, as I have shown I can write code that can fully validate user input. I decided to put all validation into this feature because I figured it would be easy to misread the instructions, or accidentally type the wrong input \(one may type the username of the winner of the game\). As well as this, columns are nicely aligned and clear, with evident separating barriers for clarity. One addition I could make, would be to show the user the games that have not been finished, as it would aid the user in keeping track of the players’ score and their position in the tournament. |
| 3 | &lt;Could also use a **code snippet** \(either a sc or plain text\) of the program when fed the input data&gt; | &lt;Either working as planned&gt; or &lt;x, y, z needed i.e \(validation of lower boundary needs correcting\)&gt; |

## Types of testing

### Black box testing

Black box testing treats the programas a black box, examining functionality without any knowledge of its internal implementation. Before you write the program create your test plan from the information given in the program specification. This is part of the design process, so black box testing is basically the test plan.

### White box testing

After you have tested your program using the test plan, look for lines of code that have not been tested. Work out extra tests for these lines of code and add the tests to the test plan.This is the white box section of a test plan. This is when you have completed the program, but added extra functions, so you have to go back to the test plan, and append data to the test plan for the new feature/lines of code. As well as appending the test log for the new lines of code.

## Lack of errors

If the final test log does not identify some program errors, either the program is a very simple one or the test plan is not rigorous enough. Normally it is the latter.

