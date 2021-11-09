# Intro to MVC

## [MVC Basics](https://www.c-sharpcorner.com/article/learn-basics-of-mvc-architecture/)

* MVC is a design pattern or architecture which helps in developing the web application in a most efficient way when compared with the traditional ASP.NET Web Application

* In traditional ASP.NET web application approach, the user action and view (UI) are combined, i.e., the web page, say, Sample.aspx and code behind Sample.aspx.cs which has the action logic are both tightly coupled, whereas in MVC, the View only deals with UI of the page and the user actions are defined in Controller

* In ASP.NET, View State is used to maintain the state of the web page. Maintaining the state means maintaining the data between post backs for a user. This makes the web page heavy which, in turn, makes the trips to server inefficient. In MVC, we don’t have View State to store the state information

* Testing is as important as development. A code which is not tested properly may break in few scenarios which degrades the quality of the software. In ASP.NET, testing is tedious task as both View (UI) and Business logic (code behind) are tightly coupled. We cannot test code-behind separately. In MVC, it enhances the test-driven development by making the UI and action logic loosely coupled. As Models, Controllers and Views are all separate layers, they can be tested easily

* 3 layers

  * Model

    * Model layer represens the objects in our Application. Model is also a class which has all the objects and its properties and methods defined in it

  * View

    * View Layer has all the html controls which define the UI of the application. Here in MVC, we don’t have drag and drop option for controls as we don’t use server controls. Instead we use Razor Engine available with Visual Studio by default which helps in rendering the View

  * Controller

    * Controller basically handles the request from user. It is the heart of the MVC application as everyone say. It is responsible to handle the request and return a response to user by loading appropriate View with data from Model

    * Controller maps the incoming user requests to appropriate Controller actions with the help of process called Routing

## [Tag Helpers](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/tag-helpers/intro?view=aspnetcore-2.1)

* What are tag helpers?

  * Tag Helpers enable server-side code to participate in creating and rendering HTML elements in Razor files

  * The built-in ImageTagHelper can append a version number to the image name. Whenever the image changes, the server generates a new unique version for the image, so clients are guaranteed to get the current image (instead of a stale cached image)

  * For the most part, Razor markup using Tag Helpers looks like standard HTML. Front-end designers conversant with HTML/CSS/JavaScript can edit Razor without learning C# Razor syntax

* Tag helpers provide:

  * An HTML friendly development experience

  * A rich IntelliSense environment for creating HTML and Razor markup

  * A way to make you more productive and able to produce more robust, reliable, and maintainable code using information only available on the server

### Additional Resources

#### [Bootstrap](https://getbootstrap.com/)

* * Some information taken from the website listed above