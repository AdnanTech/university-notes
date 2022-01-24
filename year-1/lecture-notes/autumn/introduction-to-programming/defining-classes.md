---
description: Lecture notes 06/10/2021
---

# Defining Classes

## Classes

A class describes a _kind_ of object, and specifies what sort of information the object has, called **attributes**. It specifies the operations and behaviours of the encapsulating objects, called **methods**.

Definitions of a class should be started with an upper case letter, and instances of classes should be started with a lower case.&#x20;

### Fields

Fields are **instance variables** that store values of an object within a class, for example `private int counter`.

Fields can be accessed with **getters**, called accessor methods and **setters**, called **mutator** methods.

### Constructors

Contstructors **initialise objects**, they are run immediately when an object is created, and have the same method signature as a class name, but instead it's a method.

Constructors return an instance of a class, thus they are essentially void methods, without the signature of void. So the formatting is `public className()`.

In Java, you can **overload constructors**, thus can have more than 1 constructor function, each can taking multiple or zero arguments.

## Objects

Objects are **instances** of classes. Every object has it's own attributes and methods, defined by it's class. As many objects as the memory allows can be created in Java, through using _constructor methods_.

In Java, the naming convention for classes is **upper camel case.**

## Methods & Parameters

Operations that can be **invoked** (called) for objects are called methods. Methods take parameters, and parameters have a type, and a value (even if none).

In Java, the naming convention for methods and parameters is **camel case**.

Constructors are special methods of a class, which are run automatically whenever the object is initialized. They are used to set class attributes among various other things.&#x20;

## Data types

There are lots of data types, below are some of the **primitive data types**. In C, data types come with format specifiers, depending on the data type, will determine how the data is stored in memory differently:

| Data Type                  | Format (field) Specifier | Examples (in C)                    |
| -------------------------- | ------------------------ | ---------------------------------- |
| char                       | %c                       | `printf("char var = %c", var);`    |
| signed int                 | %d / %i                  | `printf("int var = %d", var);`     |
| unsigned int               | %u                       | `printf("int var = %u", var);`     |
| short int                  | %dh / %ih                | `printf("int var = %dh", var);`    |
| float                      | %f                       | `printf("float var = %f", var);`   |
| long double                | %lf (LF) / .1lf (1 d.p)  | `printf("double var = %lf", var);` |
| double (engineer notation) | %e                       | `printf("double var = %e", var);`  |
| (string) literals          | %s                       | `printf("string var = %s", var);`  |
| bool                       | %d                       | `printf("bool var = %d\n", var);`  |
