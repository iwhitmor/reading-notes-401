# Collections & Enums

## [Collections](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/collections)

* There are two ways to group objects:

  * Arrays

  * Collections

* Collections provide a more flexible way to work with groups of objects. Unlike arrays, the group of objects you work with can grow and shrink dynamically as the needs of the application change. For some collections, you can assign a key to any object that you put into the collection so that you can quickly retrieve the object by using the key

* A collection is a class, so you must declare an instance of the class before you can add elements to that collection

* If the contents of a collection are known in advance, you can use a collection initializer to initialize the collection

* You can use a ```for``` statement instead of a ```foreach``` statement to iterate through a collection. You accomplish this by accessing the collection elements by the index position

* Some common collections:

  * System.Collections.Generic classes

  * System.Collections.Concurrent classes

  * System.Collections classes

## [Enums](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/enum)

* An enum (or enumeration type) is a value type defined by a set of named constants of the underlying integral numeric type. To define an enumeration type, use the ```enum``` keyword and specify the names of enum members

* By default, the associated constant values of enum members are of type int; they start with zero and increase by one following the definition text order. You can explicitly specify any other integral numeric type as an underlying type of an enumeration type

* The System.Enum type is the abstract base class of all enumeration types. It provides a number of methods to get information about an enumeration type and its values. For more information and examples, see the System.Enum API reference page

* Use the Enum.IsDefined method to determine whether an enumeration type contains an enum member with the certain associated value

### Additional Resources

* "C#.0 in a Nutshell": Chapter 7

* "C#.0 in a Nutshell": Pages 118-124
