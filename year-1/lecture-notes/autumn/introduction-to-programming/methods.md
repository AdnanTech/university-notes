---
description: Lecture 08/10/2021
---

# Methods

## Summary

* Methods
  * General structure
  * Accessor \(getter\) methods
  * Mutator \(setter\) methods
* Printing from methods
  * A note about "+"
* More about variables
  * Local variables

## Defining Methods

All methods have both a **header** and **body.** The header refers to the method's type signature. For example, `public int foo()` tells us that the method can be viewed and executed outside of the class, that it returns an integer, and that its name if foo and it takes zero parameters. A function with parameters is defined as such: `public int foo(int bar)` . The body of the function refers to the instructions that will be performed as part of its execution. 

### Accessors and Mutators

#### Accessors 

Accessor methods allows one to access private class attributes, perhaps with a few instructions to make sure that the value behaves in a specific way when used outside of the class. 

```text
public class Foo 
{
    private int bar; 
    public Foo(int bar)
    {
         this.bar = bar;    
    }
    // Accessor method for `bar`
    public int getBar()
    {
        return this.bar;
    }
}
```

#### Mutators 

Mutator methods allow a programmer to mutate a class attribute's value. Similarly to the previous example, there may also be some additional instructions to make sure the value is valid within the context of the class containing the attribute

```text
public class Foo 
{
    // Only expects a value greater than zero
    private int bar;
    
    public Foo(int bar)
    {
         this.bar = bar;   
    }
    
    public void setBar(int newBar)
    {
        // check to make sure the new value is greater
        // than zero, otherwise exit the function 
        if (newBar < 0) 
        {
             return ;   
        }
        this.bar = newBar;
    }
}
```

### Printing from methods

```text
public void sayHello()
{
    System.out.println("Hello, World!");
}
```

In the example above, the method `sayHello()` is a public method, which takes zero parameters, returns nothing, and simply prints `Hello, World!` to the console. The `System.out.println` method simply prints whatever parameters it takes to the screen, typically `stdout` , it typically expects a string. For formatted output \(think `printf` from C\) you can use `System.out.printf` with the same format specifiers as printf. 

When formatting lines, the concatenation operator is used \("+"\). This simply combines two strings together. If a non-string value is provided, it will be converted to a string. When working with this operator, be careful with spaces, as by default, it does not append any whitespace between the concatenated values. 

### Local variables

When writing the body of a function, you may find yourself needing to declare new variables within the body. However, once the method exists, the variables are dropped from memory, meaning you will not be able to access them again. If you want to use them again however, one variable can be returned from the method and used in another method, such as in the main function. 

