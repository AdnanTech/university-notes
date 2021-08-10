# Macros \(headers\)

## Macros

Macros are like the c equivalent of constant, global variables.

The C preprocessor is a macro preprocessor \(allows you to define macros\) that transforms your program before it is compiled. These transformations can be the inclusion of header file, macro expansions etc.

All preprocessing directives begin with a `#` symbol. For example

### Object-like macros

You can define to use constants, for example: `#define c 299792458` , which is speed of light. The number is a literal. This means that it has an implicit data type. _That is processed during compilation?_ asd

### Function like macros

`#define circleArea(r) (3.1415(r)(r))` These are functions that are defined that we can reuse.

