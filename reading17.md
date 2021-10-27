# MVC Forms

## [View Models](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/overview?view=aspnetcore-5.0&viewFallbackFrom=aspnetcore-2.2)

* In the Model-View-Controller (MVC) pattern, the view handles the app's data presentation and user interaction

* A view is an HTML template with embedded Razor markup. Razor markup is code that interacts with HTML markup to produce a webpage that's sent to the client

* In ASP.NET Core MVC, views are .cshtml files that use the C# programming language in Razor markup. Usually, view files are grouped into folders named for each of the app's controllers. The folders are stored in a Views folder at the root of the app

* ***Layouts***

  * provide consistent webpage sections and reduce code repetition. Layouts often contain the header, navigation and menu elements, and the footer. The header and footer usually contain boilerplate markup for many metadata elements and links to script and style assets. Layouts help you avoid this boilerplate markup in your views

* ***Partial Views***

  * Reduce code duplication by managing reusable parts of views. For example, a partial view is useful for an author biography on a blog website that appears in several views

* ***View Components***

  * Similar to partial views in that they allow you to reduce repetitive code, but they're appropriate for view content that requires code to run on the server in order to render the webpage. View components are useful when the rendered content requires database interaction, such as for a website shopping cart

* ***Benefits of using Views***

  * The app is easier to maintain because it's better organized. Views are generally grouped by app feature. This makes it easier to find related views when working on a feature

  * The parts of the app are loosely coupled. You can build and update the app's views separately from the business logic and data access components. You can modify the views of the app without necessarily having to update other parts of the app
  
  * It's easier to test the user interface parts of the app because the views are separate units.
  Due to better organization, it's less likely that you'll accidentally repeat sections of the user interface

## [4 Ways to make a form in .NET MVC](https://www.completecsharptutorial.com/asp-net-mvc5/4-ways-to-create-form-in-asp-net-mvc.php)

* Forms are very essential and basic thing that every programmer has to learn

* There are four different ways to create forms in ASP.NET MVC

  * ***Weakly Typed (Synchronous)***
  
    * Weakly typed forms are the easiest forms to create in MVC

    * Mostly used when you need to create a form with one or two input items

  * ***Strongly Typed (Synchronous)***

    * In this method, we send objects (model) instead of sending each item as parameter. It is easy to maintain because you don't need to remember each input item and IntelliSense will show you automatically the each item

  * ***Strongly Typed AJAX (Asynchronous)***

    * Asynchronous AJAX form is a very magical way to submit data to the controller without happening page load. Asynchronous AJAX Forms simply post back the data to the controllers and update the only that part of the page, which has to display output

    * To make this happen, we will use JQuery-Unobstrusive-AJAX. This is a great feature which is launched in MVC 3. It helps you to create AJAX Form without writing bunch of javascript code

  * ***HTML, AJAX and JQUERY***

    * In this method, you can not only send data from input controls but can also use html elements like ```<p>```, ```<\p>```, ```<span>```, and ```<\span>``` to send data to controllers. This is pure JQuery and AJAX query

### Additional Resources

* Some information taken from the linkes provided above
