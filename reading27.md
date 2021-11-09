# MVC Forms

## [View Models](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/overview?view=aspnetcore-6.0&viewFallbackFrom=aspnetcore-2.2)

* In MVC the VIEW handles the apps data and presentation to the user

* The VIEW is an HTML template with razor markup. Razor markup is code that interacts with HTML to produce the webpage

* All VIEW files are .cshtml and written in C#

* VIEW files are grouped into folders named for each of the app's controllers. The folders are stored in a Views folder at the root of the app

* Benefits to using views

  * The app is easier to maintain because it's better organized. Views are generally grouped by app feature. This makes it easier to find related views when working on a feature

  * The parts of the app are loosely coupled. You can build and update the app's views separately from the business logic and data access components. You can modify the views of the app without necessarily having to update other parts of the app

  * It's easier to test the user interface parts of the app because the views are separate units

  * Due to better organization, it's less likely that you'll accidentally repeat sections of the user interface

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

* Some information taken from the website listed above