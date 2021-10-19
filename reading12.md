# Entity Framework and APIs

## [Entity Framework Core](https://docs.microsoft.com/en-us/ef/core/)

* Entity Framework (EF) Core is a lightweight, extensible, open source and cross-platform version of the popular Entity Framework data access technology

* EF Core can serve as an object-relational mapper (O/RM), which:

  * Enables .NET developers to work with a database using .NET objects

  * Eliminates the need for most of the data-access code that typically needs to be written

* The Model

  * Data access is is performed using a model

  * A model is made up of entity classes and a context object that represents a session with the database

  * Entity framework supports the following model development:

    * Generate a model from an exisiting framework

    * Hand code a model to match the database

* Data is created, deleted, and modified in the database using instances of your entity classes

## [Data Seeding](https://docs.microsoft.com/en-us/ef/core/modeling/data-seeding)

* Data seeding is the process of populating a database with an initial set of data

* Several ways to do this:

  * Model seed data

  * Manual migration customization

  * Custom initialization logic

## [User Secrets](https://codefellows.github.io/code-401-dotnet-guide/resources/user-secrets.html)

* User secrets is a secure way of storing private user information such as API keys, client secrets, and connection strings (things you don't want others to know about)

### Additional Resources

* Some information taken from the linkes provided above

[Intro to APIs](https://www.youtube.com/watch?v=aIkpVzqLuhA)

[MVC with EF Get Started](https://docs.microsoft.com/en-us/aspnet/core/data/ef-mvc/intro?view=aspnetcore-5.0)