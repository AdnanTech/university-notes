# Files

Files provide backup storage for data, normally on a physical disk. When a program is terminated, the entire data stored in memory is lost. Using files allows data to be easily moved from one computer to another.

Text files are stored as strings of readable characters. Notepad.txt files, C .c source code filesand HTML .html files are examples of text files. Binary files are used to store binary formatted data such as photo .jpeg files, compressed data .zip files and lecture notes .pdf files

## Working with Files

When working with files, you need to declare a pointer of type FILE and then initialise it with fopen\(\). This pointeris needed for communication between the file and program

```c
/* Code to access files */

FILE *fptr; /* Create the pointer to the file */
fptr = fopen("filename", "fileMode"); 
```

|  File Mode | Defiinition | If file does not existr |
| :--- | :--- | :--- |
| r | Open file for reading | If does not exist, fopen\(\) returns NULL |
| rb | Open file for reading in binary mode | If does not exist, fopen\(\) returns NULL |
| w | Open file for writing | If the file exists, its contents are overwritten. If the file does not exist, it will be created. |
| wb | Open file for writing in binary mode | If the file exists, its contents are overwritten. If the file does not exist, it will be created. |
| a | Open file for append | If the file does not exist, it will be created |
| ab | Open file for append in binary mode | If the file does not exist, it will be created |
| r+ | Open file for both reading and writing | If does not exist, fopen\(\) returns NULL |
| rb+ | Open file for both reading and writing in binary mode | If does not exist, fopen\(\) returns NULL |
| w+ | Open file for both reading and writing | If the file exists, its contents are overwritten. If the file does not exist, it will be created. |
| wb+ | Open file for both writing and writing in binary mode | If the file exists, its contents are overwritten. If the file does not exist, it will be created. |
| a+ | Open file for both reading and appending | If the file does not exist, it will be created |
| ab+ | Open file for both reading and appending in binary mode | If the file does not exist, it will be created |

## File functions

Just like how in normal C there are functions like getchar\(\), putchar\(\), scanf\(\) and print\(\), the equivalent exists for file input and output functions

| Function | Usage |
| :--- | :--- |
| fgetc\(\) | Gets the next character \(an unsigned char\) from the specified stream and advances the position indicator for the stream |
| fputc\(\) | Writes a character \(an unsigned char\) specified by the argument **char** to the specified stream and advances the position indicator for the stream |
| fscanf\(\) | Reads formatted input from a stream |
| fprintf\(\) | Sends formatted output to a stream |

## [Examples are in the code base](https://adnantech.gitbook.io/code/code/c/files)

