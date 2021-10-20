# Dependency Injection

## [Dependency Injection](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/dependency-injection?view=aspnetcore-5.0)

ASP.NET Core supports the dependency injection (DI) software design pattern, which is a technique for achieving Inversion of Control (IoC) between classes and their dependencies

* Dependency Injection

  * A dependency is an object that another object depends on

  * A class can create an instance of the MyDependency class to make use of its WriteMessage method

  * The class creates and directly depends on the MyDependency class. Code dependencies are problematic and should be avoided for the following reasons:

    * To replace MyDependency with a different implementation, the IndexModel class must be modified.

    * If MyDependency has dependencies, they must also be configured by the IndexModel class. In a large project with multiple classes depending on MyDependency, the configuration code becomes scattered across the app.

    * This implementation is difficult to unit test. The app should use a mock or stub MyDependency class, which isn't possible with this approach.

  * Dependency injection addresses these problems:

    * The use of an interface or base class to abstract the   dependency implementation.

    * Registration of the dependency in a service container. ASP.NET Core provides a built-in service container, IServiceProvider. Services are typically registered in the app's Startup.ConfigureServices method.

    * Injection of the service into the constructor of the class where it's used. The framework takes on the responsibility of creating an instance of the dependency and disposing of it when it's no longer needed.

## [Repository Pattern](https://docs.microsoft.com/en-us/dotnet/architecture/microservices/microservice-ddd-cqrs-patterns/infrastructure-persistence-layer-design#the-repository-pattern)

The Repository Pattern

* The repository pattern is a well-documented way of working with a data source

* Repositories are classes or components that encapsulate the logic required to access data sources. They centralize common data access functionality, providing better maintainability and decoupliing the infrastructure or tech used to access databases from the domain model layer

* The repository pattern allows you to easily test your app with unit tests

## [Repository Design Pattern](https://medium.com/@pererikbergman/repository-design-pattern-e28c0f3e4a30)

The repository pattern has two purposes:

1. It is an abstraction of the data layer
2. It is a way of centralising the handling of the domain objects

## [SOLID Principles](https://www.telerik.com/blogs/30-days-of-tdd-day-five-make-your-code-solid)

Single Responsibility Principle

* The idea that every mthod or class in your app should have exactly one reason to change or that every class or method in your app sould have exactly one job or responsibility

The Open/Close Principle

* Software should be open for extension, but closed to modification

The Liskov Substitution Principle

* An object in your app should be able to be replaced with a type derived from it without breaking the app.

The Interface Segregation Principle

* Clients should not be forced to rely on interfaces they do not use

The Dependency Inversion Principle

* Code should depened on abstractions; not concrete implementations. Furthermore, those abstractions should not depend on the details; the details should depend on the abstractions

## [Why SOLID Matters](https://www.telerik.com/blogs/why-solid-matters)

It helps when you are testing/writing tests. You can change/refactor your code so that it does the one thing that it is supposed to do, and is still clean and consise

## [SOLID Principles in Pictures](https://medium.com/backticks-tildes/the-s-o-l-i-d-principles-in-pictures-b34ce2f1e898)

Single Responsibility

<img src="https://miro.medium.com/max/2000/1*P3oONz9Da3Tc1w97fMV73Q.png" />

Open-Closed

<img src="https://miro.medium.com/max/2000/1*0MtFBmm6L2WVM04qCJOZPQ.png" />

Liskov Substitution

<img src="https://miro.medium.com/max/2000/1*yKk2XKJaCLNlDxQMx1r55Q.png" />

Interface Segregation

<img src="<https://miro.medium.com/max/5200/1*2hmyR9L43Vm64MYxj4Y89w.png> />

Dependency Inversion

<img src="https://miro.medium.com/max/2000/1*Qk8tDmjQlyvwKxNTfXIo0Q.png" />

### Additional Resources

Some information taken from the links provided above
