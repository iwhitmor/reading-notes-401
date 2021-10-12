# Interfaces

## [Interfaces](https://docs.microsoft.com/en-us/dotnet/csharp/fundamentals/types/interfaces)

* An interface contains definitions for a group of related functionalities that a non-abstract class or a struct must implement

* An interface may define ```static``` methods, which must have an implementation

* By using them, you can include behavior from multiple sources in a class. That capability is important because the language doesn't support multiple inheritance of classes

* You define an interface by using the ```interface``` keyword. The name of an interface must be a valid C# identifier name. They conventionally begin with a capital ```I```

* Interfaces can contain instance methods, properties, events, indexers, or any combination of those four member types. Interfaces may contain static constructors, fields, constants, or operator

* A class or struct can implement multiple interfaces. A class can inherit a base class and also implement one or more interfaces.

## [Back to basics](https://simpleprogrammer.com/back-to-basics-what-is-an-interface/)

* The basic problem an interface is trying to solve is to separate how we use something from how it is implemented

* We do this so we can write code that can work with a variety of different implementations of some set of responsibilities without having to specifically handle each implementation

* Interfaces allow us to specify that a particular class meets certain expectations that other classes can rely on

## [Interfaces #2](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/interface)

* An interface defines a contract

* Any class or struct that implements that contract must provide an implementation of the members defined in the interface

* It may also define static members in order to provide a single implementation for common functionality

* An interface declaration can contain declarations of the following members:

  * Methods

  * Properties

  * Indexers

  * Events

* An interface may include:

  * Constants

  * Operators

  * Static constructor

  * Nested types

  * Static fields

  * Methods
  
  * Properties

  * Indexers

  * Events

  * Member declarations using the explicit interface syntax

  * Explicit access modifiers

### Additional Resources

* Information taken from the links that are provided above
