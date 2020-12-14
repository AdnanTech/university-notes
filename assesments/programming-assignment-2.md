# Programming Assignment 2

{% file src="../.gitbook/assets/progproj2.pdf" caption="Project Brief" %}

{% file src="../.gitbook/assets/stylerulesc.pdf" caption="Style Rules" %}

## Scoping

Project consists of two programs:

## Program 1

A program that allows one of their volunteers to enter trial participant details into a computer file prior to the trial participant being seen by a research doctor for the vaccine injection.

### The volunteers

* There are 5 volunteers: Bill Gates, Boris Johnson, Mark Drakeford, Nicola Sturgeon and Arlene Foster. They enter the participant details.
* Only these 5 volunteers can access the first program, they are each given an login id and a password.
* _Passwords are to be exactly 7 characters in length_.
* Each password has a _seven character caesar cipher encryption_, that wraps around, so “aBc2xyz8” becomes “hLj9efg5”.
* The ids and encrypted _passwords should be stored in arrays in memory_.

Then, the volunteer will write the participant's data to a file, this includes the participants:

* First name
* Last name
* Date of birth
* Height
* Weight
* Medical conditions
* Current medication
* Vaccine code number \(a unique 9 digit number\)
* Additional comment

Each trial participant’s details will be written to a file and encrypted using the same algorithm that was used for the passwords. Punctuation and spaces remain unencrypted. The name of the file will be the trial participant’s last name, plus their date of birth as 6 digits with an extension of “.mxa” eg “smith010285.mxa”.

## Program 2

A program that allows the research doctor to read and update a trial participant’s files.

### The Research Doctors

* The research doctor, Michel Barnieror David Frost, should have a password to log into the second program.
* After logging in, Michel or David should enter the trial participant’s last name and date of birth.
* The program will then read the appropriate file and present the trial participant’s details in a readable form on the screen.
* The research doctor should then enter the vaccine code number and any additional comments to the trial participant’s notes before resaving the data to the file.
* Additionally, when either program starts, the stored ids and encrypted passwords should be read from a password file.
* Any maintenance of ids or passwords should be done by the research doctor in the second program.
* The research doctor should be allowed to add, delete or change any volunteers’ id or password.
* When the research doctor’s program finishes the password file should be overwritten with the updated stored ids and encrypted passwords.

## Limitations

* Stored IDs when updated, can overwrite another volunteer's IDs, as I have not implemented any validation

## Assumptions

* We assume to volunteer to participant ratio is one to one

