# View Components

## [Intro to View Components](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/view-components?view=aspnetcore-2.1)

* View components are similar to partial views, but they're much more powerful. View components don't use model binding, and only depend on the data provided when calling into it

* A view component:

  * Renders a chunk rather than a whole response

  * Includes the same separation-of-concerns and testability benefits found between a controller and view

  * Can have parameters and business logic

  * Is typically invoked from a layout page

* View components are intended anywhere you have reusable rendering logic that's too complex for a partial view, such as:

  * Dynamic navigation menus

  * Tag cloud (where it queries the database)

  * Login panel

  * Shopping cart

  * Recently published articles

  * Sidebar content on a typical blog

  * A login panel that would be rendered on every page and show either the links to log out or log in, depending on the log in state of the user

* A view component consists of two parts:

  * Class (derived from the view component)

  * Result it returns (a view)

* Creating a View Component

  * Deriving from ViewComponent

  * Decorating a class with the [ViewComponent] attribute, or deriving from a class with the [ViewComponent] attribute

  * Creating a class where the name ends with the suffix ViewComponent

## [View Components](https://mariusschulz.com/blog/view-components-in-asp-net-core-mvc)

* View components were introduced in ASP.NET MVC 6

* Summary of view components from ASP.NET documentation:

  * View components include the same separation-of-concerns and testability benefits found between a controller and view. You can think of a view component as a mini-controller—it’s responsible for rendering a chunk rather than a whole response. You can use view components to solve any problem that you feel is too complex with a partial

* Writing a view component

  * Like controllers, view components must be public, non-nested, and non-abstract classes that either:

    * Derive from the ViewComponent class

    * Are decorated with the [ViewComponent] attribute, or have a name that ends with the "ViewComponent" suffix

* ASP.NET MVC 6 introduces view components, a component-oriented mixture of child actions and partial views. They can return various content, including Razor views, JSON, or plain text

* View components can be rendered synchronously or asynchronously

* View components can integrate with the dependency injection system of ASP.NET Core through constructor injection

### Additional Resources

Some information taken from the links provided above

