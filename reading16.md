# Data Transfer Objects

## [Data Transfer Objects](https://docs.microsoft.com/en-us/aspnet/web-api/overview/data/using-web-api-with-entity-framework/part-5)

A DTO (Data Transfer Object) is an object that defines how the data will be sent over the network

Sometimes you might want to change the shape of the data you sent. You can do this in a couple of different ways

* Remove circular references (see previous section)

* Hide particular properties that clients are not supposed to view

* Omit some properties in order to reduce payload size

* Flatten object graphs that contain nested objects, to make them more convenient for clients

* Avoid "over-posting" vulnerabilities. (See Model Validation for a discussion of over-posting)

* Decouple your service layer from your database layer

## [How to Use DTOs](https://www.infoworld.com/article/3562271/how-to-use-data-transfer-objects-in-aspnet-core-31.html)

* The biggest advantage of using DTOs is decoupling clients from your internal data structures

* When designing and developing an application, if you’re using models to pass data between the layers and sending data back to the presentation layer, then you’re exposing the internal data structures of your application. That’s a major design flaw in your application

* By decoupling your layers DTOs make life easier when you’re implementing APIs, MVC applications, and also messaging patterns such as Message Broker

* You can take advantage of DTOs to abstract the domain objects of your application from the user interface or the presentation layer. In doing so, the presentation layer of your application is decoupled from the service layer

* Another reason you would want to use DTOs is data hiding. That is, by using DTOs you can return only the data requested

* A DTO is meant to transport data from one layer of an application to another layer. The consumer of a DTO might be built in .NET/C#/Java or even JavaScript/TypeScript. A DTO is often serialized so that it can be independent of the technology used in the receiver

* Data Transfer Objects typically don’t contain any business logic — they only contain data. Immutability is a desired feature when working with DTOs. There are several ways in which you can implement immutable DTOs

### Additional Resources

Some information taken from the links provided above
