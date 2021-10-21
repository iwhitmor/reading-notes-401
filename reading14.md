# Navigation Properties and Routing

## [Routing within MVC](https://docs.microsoft.com/en-us/aspnet/mvc/overview/older-versions-1/controllers-and-routing/asp-net-mvc-routing-overview-cs)

* The ASP.NET Routing module is responsible for mapping incoming browser requests to particular MVC controller actions
* When you create a new ASP.NET MVC application, the application is already configured to use ASP.NET Routing
* ASP.NET routing it set up in two places
  * 1. ASP.NET Routing is enabled in your application's Web configuration file (Web.config file)
    * Four sections in the config file that are relevant
      * 1. system.web.httpModules section
      * 2. system.web.httpHandlers section
      * 3. system.webserver.modules section
      * 4. system.webserver.handlers section
  * 2. W route table is created in the application's Global.asax file. The Global.asax file is a special file that contains event handlers for ASP.NET application lifecycle events. The route table is created during the Application Start event
* When an MVC application first starts, the Application_Start() method is called. This method, in turn, calls the RegisterRoutes() method. The RegisterRoutes() method creates the route table

## [Routing within Core](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/routing?view=aspnetcore-3.1)

* Routing is responsible for matching incoming HTTP requests and dispatching those requests to the app's executable endpoints
* Endpoints are the app's units of executable request-handling code
* Endpoints are defined in the app and configured when the app starts
* The endpoint matching process can extract values from the request's URL and provide those values for request processing. Using endpoint information from the app, routing is also able to generate URLs that map to endpoints.
* Apps can configure routing by:
  * Controllers
  * Razor Pages
  * SignalR
  * gRPC Services
  * Endpoint-enabled middleware such as Health Checks
  * Delegates and lambdas registered with routing
* Routing uses a pair of middleware, registered by UseRouting and UseEndpoints: 
  * ```UseRouting```
  * ```UseEndpoints```
* The ```MapGet``` method is used to define an endpoint
* An endpoint is something that can be selected by matching the HTTP method and the URL and also can be executed, by running the delegate
* URL matching
  * Is the process by which routing matches an incoming request to an endpoint.
  * Is based on data in the URL path and headers.
  * Can be extended to consider any data in the request
* URL generation concepts
  * Is the process by which routing can create a URL path based on a set of route values
  * Allows for a logical separation between endpoints and the URLs that access them

### Additional resources

* Some information taken from the reading above