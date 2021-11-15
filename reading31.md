# Razor Pages

## [Razor Pages](https://gunnarpeipman.com/aspnet-core-razor-pages/)

* Why Razor Pages?

  * It’s easier to get to web development for beginners as Razor pages are more lightweight than MVC. Besides beginners there are people who are coming from other scripting languages be it old ASP or PHP or something else

  * Razor Pages fit well to smaller scenarios where building controllers and models as separate classes is overkill

* What are they?

  * App structure is dimilar to MVC, but there are no folders for controllers and views

  * Program and Startup classes are exactly the same as for MVC applications. Not just by name but also by code

  * Razor pages are a "lightweight" option for those who just want to get started with ASP.NET

## [Razor Pages vs MVC](https://jonhilton.net/razor-pages-or-mvc-a-quick-comparison/)

* With Razor Pages, when you make a request (e.g. /contact) the default ASP.NET Routing configuration will attempt to locate a Razor Page for that request in the Pages folder

* It simply looks for a page with the name used in the request (for a request to /contact that would be Contact.cshtml) and routes directly to it

  * The Razor Page then acts as though it were a controller action

* Every razor page can have a corresponding page model

* The default routing for Razor Pages is simple enough and respects subfolders, so a route  would be accessible via a request to profile

* Rather than have separate ViewModels you just need to add properties to your Page Model and you can directly set those properties from your Page Model methods (e.g. OnGet)

* Everything lives in the PAGES FOLDER (by default)

* Each Razor Page consists of the View template (.cshtml) and a corresponding .cs file which effectively acts as a controller action, specifically for that view

### Additional Resources

#### [Getting started with Razor Pages](https://docs.microsoft.com/en-us/aspnet/core/tutorials/razor-pages/razor-pages-start?view=aspnetcore-2.1&tabs=visual-studio)

#### [Razor Pages](https://docs.microsoft.com/en-us/aspnet/core/razor-pages/?view=aspnetcore-2.2&tabs=visual-studio)

##### Some informatin taken from the links listed above
