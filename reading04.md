# Classes & Memory Management

## [Classes](https://docs.microsoft.com/en-us/dotnet/csharp/fundamentals/types/classes)

* Reference Types

  * A type that is defined as a class is a reference type. At run time, when you declare a variable of a reference type, the variable contains the value null until you explicitly create an instance of the class by using the new operator, or assign it an object of a compatible type that may have been created elsewhere

* Declaring Classes

  * You declare a class by using the ```class``` keyword followed by a unique identifier. The ```class``` keyword is preceded by the access level. The name of the class follows the ```class``` keyword and the name of the ```class``` must have a C# identifier

* Creating Objects

  * Object is an entity based on the class. Objects are created using the ```new``` keyword followed by the name of the class that the object will be based on

* Class Inheritance

  * Classes fully support inheritance, a fundamental characteristic of object-oriented programming. When you create a class, you can inherit from any other class that is not defined as sealed, and other classes can inherit from your class and override class virtual methods. Furthermore, you can implement one or more interfaces.

## [Constructors](https://canvas.instructure.com/courses/3478514/discussion_topics/12575584)

* Whenever a class or struct is created, its constructor is called. A class or struct may have multiple constructors that take different arguments. Constructors enable the programmer to set default values, limit instantiation, and write code that is flexible and easy to read.

* Static Constructors

  * A class or struct can also have a static constructor, which initializes static members of the type. Static constructors are parameterless

## [Properties](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/properties)

* A property is a member that provides a flexible mechanism to read, write, or compute the value of a private field. Properties can be used as if they are public data members, but they are actually special methods called accessors. This enables data to be accessed easily and still helps promote the safety and flexibility of methods.

* Properties enable a class to expose a public way of getting and setting values, while hiding implementation or verification code.

* A get property accessor is used to return the property value, and a set property accessor is used to assign a new value

* The value keyword is used to define the value being assigned by the set or init accessor.

## [Stack and Heap](https://www.c-sharpcorner.com/article/C-Sharp-heaping-vs-stacking-in-net-part-i/)

* Both the stack and heap help us run our code.  They reside in the operating memory on our machine and contain the pieces of information we need to make it all happen.

* Stack

  * The stack is responsible for keeping track of what is executing in our code

  * The stack is self-maintaining. Meaning it takes care of its own memory management

* Heap

  * The heap is responsible for keeping of our objects

  * The heap has to worry about garbage collection (GC) which deals with how to keep the heap clean

* Value Types

  * In C#, all the "things" declared with the following list of type declarations are Value types (because they are from System.ValueType)
    * bool
    * byte
    * char
    * decimal
    * double
    * enum
    * float
    * int
    * long
    * sbyte
    * short
    * struct
    * uint
    * ulong
    * ushort

* Reference types

  * All the "things" declared with the types in this list are Reference types (and inherit from System.Object... except, of course, for object which is the System.Object object):
    * class
    * interface
    * delegate
    * object
    * string

* Pointers

  * A reference is often referred to as a POINTER. They are managed by the CLR. A pointer is a chunk or space of memory that points to another space of memory

* Instructions

  * Tells our code what to do (execut a method etc)

## [Garbage Collection Fundamentals](https://docs.microsoft.com/en-us/dotnet/standard/garbage-collection/fundamentals)

* In the common language runtime (CLR), the garbage collector (GC) serves as an automatic memory manager

* The garbage collector manages the allocation and release of memory for an application

* Benefits

  * Frees developers from having to manually release memory

  * Allocates objects on the managed heap efficiently

  * Reclaims objects that are no longer being used, clears their memory, and keeps the memory available for future allocations. Managed objects automatically get clean content to start with, so their constructors don't have to initialize every data field

  * Provides memory safety by making sure that an object cannot use for itself the memory allocated for another object

* Fundamentals of memory

  * Each process has its own, separate virtual address space. All processes on the same computer share the same physical memory and the page file, if there is one

  * Virtual memory can be in 3 different states:

    * Free

    * Reserved

    * Committed

  * You can run out of memory if there isn't enough virtual address space to reserve or physical space to commit

* Memory Allocation

  * Allocating memory from the managed heap is faster than unmanaged memory allocation. Because the runtime allocates memory for an object by adding a value to a pointer, it's almost as fast as allocating memory from the stack

* The managed heap

  * After the garbage collector is initialized by the CLR, it allocates a segment of memory to store and manage objects. This memory is called the managed heap, as opposed to a native heap in the operating system

### Additional Resources

* Chapter 3 from C# In A Nutshell

* Information taken from links provided above
