# Object Oriented

## The Basics

Object Oriented can be broken down into Object Oriented Analysis \(OOA\), Object Oriented Design \(OOD\) and Object Oriented Programming \(OOP\).

### Key Terms

**Object:** An object is an **instance** of a **class** \(derived from classes\) or a **variable \(fields\)** that defines data and behaviour**.** An object can be a combination of variables, functions and data structures.

**Attribute:** An attribute is **property** or **member variable.** Attributes are data elements of objects, so they store data inside a class or instance, about the instance. Is also pretty much equivalent to a **field**.

**Class:** A class is a **blueprint** for defining **objects'** attributes and operations**.** Classes allow for **abstract data types**.

**Operation:** An action performed by an object. Essentially a **method** or **member function**.

**Assess methods:** allow attribute data to be seen by code outside the class of objects.

**Mutation methods:** allow attribute data to be changed by code outside the class.

**Aggregation and Composition**: An object containing an embedded object.

**Association and Collaboration**: Messages are used to link objects of different classes.

**Use Case**: A goal a user has in using the system.

## What makes OOP

The key concept for the Object Oriented approach to programming is the **relationship** between **classes** and **objects.**

### Polymorphism

Polymorphism is where an object can take on different forms. Forms refers to states, a real life of an example is that the object can be a person, who has many different characteristics, uni student, working and a caring brother. In OOP, an example of oplymorphism is where a parent class makes a reference to a child class object.

A function with different implementations depending on the object type or list of parameters. Also known as function overloading or operator overloading. Constructors are also good examples of polymorphism.

### Inheritance

Inheritance is where attributes and methods of a class are inherited from another class.

Generalisation and specialisation, Parent and child, super class and subclass, and base class and derived class. An example of this would be to have a base class called vehicle and a derived class called car.

### Abstraction

**Abstracting** data is to **reduce complexity** by removing unnecessary information. This means thinking of programming using objects in a machine esque kind of way.

A key example of abstraction is an **API** \(Application Programming Interface\), more commonly known as a **library**. An interface is a set of public **assess** and **mutation methods** in an object A **package** is a **namespace** that organizes a set of related classes and interfaces.

### Encapsulation

Modularity is closely tied with encapsulation and classes. The C++ convention is to create two files for each class of objects. A header file .h for the class definition. An implementation file .cppfor the code of the class methods.

Data hiding, prevents unintended or malicious changes by ensuring exclusivity of data acess to class members. Generally, you'll want to privatise the attributes, and publicise the methods, for re use.

#### Reuse

Re use often refers to using inheritance in your application to take advantage of behaviour implemented in existing classes. Inheritance is one of the fundamental concepts of object orientation, letting you model “is a”, “is like”, and “is kind of” relationships. Re use of class libraries is also one of the main goals behind the invention of object oriented programming.

## Constructors & Destructors

A **constructor** is a special method, with the same name as its class, which is called to **create an object**. It is normally used to initialise the attributes of the object. It can have parameters but does not have a return type.

A **destructor** in C++ is a method, with its name starting with '~' followed by the class name, which is automatically **invoked when the object is destroyed**. It does not have parameters or a return type. Destroyed refers to when an object is out of scope or called to be deleted.

To expand on when the destructor is called. It is called after all the funcitons in the class are run AND the code is out of scope, meaning _after the function has been ran to completion, or after the block of code._

## Object Oriented Analysis Design

**UML**: **Unified Modelling Language**, a set of defined diagrams for doing OOAD \(Object Oriented Analysis Design\). These include Use Case diagrams, Class diagrams and Sequence diagrams.

**RUP**: **Rational Unified Process**, a system development life cycle.

