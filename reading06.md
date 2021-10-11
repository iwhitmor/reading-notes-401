# Object Oriented Principles

## [Inheritance](https://docs.microsoft.com/en-us/dotnet/csharp/fundamentals/object-oriented/inheritance)

* Inheritance is one of the three primary characteristics of object-oriented programming

* It enables you to create new classes that reuse, extend, and modify the behavior defined in other classes

* Base Class = the class whose members are inherited

* Derived Class = the class that inherits those members

  * A derived class can have only one direct base class

* Inheritance is transitive

  * If ```ClassC``` is derived from ```ClassB```, and ```ClassB``` is derived from ```ClassA```, ```ClassC``` inherits the members declared from ```ClassB``` and ```ClassA```

## [Abstract](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/abstract-and-sealed-classes-and-class-members)

* The ```abstract``` keyword enables you to create classes and class members that are incomplete and must be implemented in a derived class

* Classes can be declared as abstract by puttin gthe keyword ```abstract``` before the class definition

  * For example: ```public abstract class A```

* An abstract class cannot be instantiated. The purpose of an abstract class is to provide a common definition of a base calss that multiple derived classes can share

* They can also define abstract methods. You can do this by adding the ```abstract``` keyword before the return type of a method

  * For example: ```public abstract void DoWork(int i);``` 

## [Polymorphism](https://docs.microsoft.com/en-us/dotnet/csharp/fundamentals/object-oriented/polymorphism)

* At run time, objects of a derived class may be treated as objects of a base class in places such as method parameters and collections or arrays. When this polymorphism occurs, the object's declared type is no longer identical to its run-time type

* Base classes may define and implement virtual methods, and derived classes can override them, which means they provide their own definition and implementation. At run-time, when client code calls the method, the CLR looks up the run-time type of the object, and invokes that override of the virtual method. In your source code you can call a method on a base class, and cause a derived class's version of the method to be executed

## [OOP Principles](https://docs.microsoft.com/en-us/dotnet/csharp/fundamentals/tutorials/oop)

* The four basic principles of object-oriented programming are:

  * Abstraction: Modeling the relevant attributes and interactions of entities as classes to define an abstract representation of a system

  * Encapsulation: Hiding the internal state and functinality of an object and only allowing access through a public set of functions

  * Inheritance: Ability to create new abstractions based on existing abstractions

  * Polymorphism: Ability to implement inherited properties or methods in different ways across multiple abstractions

### Additional Resources

* Chapter 3 from "C# in a Nutshell"

* Information taken from links provided above