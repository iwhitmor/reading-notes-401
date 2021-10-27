# Identity / Authentication

## [Intro To Identity](https://docs.microsoft.com/en-us/aspnet/core/security/authentication/identity?view=aspnetcore-5.0&tabs=visual-studio)

* ***ASP.NET Core Identity***

  * Is an API that supports user interface (UI) login functionality

  * Manages users, passwords, profile data, roles, claims, tokens, email confirmation, and more

  * Users can create an account with the login information stored in Identity or they can use an external login provider. Supported external login providers include Facebook, Google, Microsoft Account, and Twitter

  * Identity is typically configured using a SQL Server database to store user names, passwords, and profile data. Alternatively, another persistent store can be used, for example, Azure Table Storage

* ***Microsoft Identity Platform***

  * An evolution of the Azure Active Directory (Azure AD) developer platform

  * Unrelated to ASP.NET Core Identity

* ***Identity Components***

  * All the Identity-dependent NuGet packages are included in the ASP.NET Core shared framework

  * The primary package for Identity is Microsoft.AspNetCore.Identity. This package contains the core set of interfaces for ASP.NET Core Identity, and is included by Microsoft.AspNetCore.Identity.EntityFrameworkCore

## [Identity Demystified](https://digitalmccullough.com/blog/aspnetcore-auth-system-demystified/)

* There is a component, AUTHENTICATION SYSTEM, in ASP.Net that protects your website/app from unauthorized usage and access

* Understanding the system first requires understanding its components and behaviors. They can be broken down into identity, verbs, authentication handlers, and middleware

* ***Identity***

  * There are three classes which represent the identity of the user:

    * Claims

      * A Claim represents a single fact about the user. It could be the user's first name, last name, age, employer, birth date, or anything else that is true about the user. A single claim will contain only a single piece of information

    * ClaimsIdentity

      * An Identity represents a form of identification or, in other words, a single way of proving who you are. In real life this could be a driver's license. In ASP.Net Core, it is a ClaimsIdentity. This class represents a single form of digital identification

    * ClaimsPrincipal

      * A Principal represents the actual user. It can contain one or more instances of ClaimsIdentity, just like in life a person may have a driver's license, concealed-carry permit, social security card, and a passport. Each of the identities is used for a different purpose and may contain a unique set of claims, but they all identify the same user in some form or another
  
* ***Verbs***  
  
  * There are five verbs that are invoked by the auth system:

    * Authenticate

      * Gets the user’s information if any exists

    * Challenge

      * Requests authentication by the user

    * SignIn

      * Persists the user’s information somewhere

    * SignOut

      * Removes the user’s persisted information

    * Forbid

      * Denies access to a resource for unauthenticated users or authenticated but unauthorized users
  
* ***Authentication Handlers***

  * Authentication handlers are components that actually implement the behavior of the 5 verbs above. The default auth handler provided by ASP.NET Core is the Cookies authentication handler which implements all 5 of the verbs

  * Authentication handlers must be registered with the auth system in order to be used and are associated with schemes. A scheme is just a string that identifies a unique auth handler in a dictionary of auth handlers

* ***Authentication Middleware***

  * A middleware is a module that can be inserted into the startup sequence and is run on every request

  * This code checks if a user is authenticated (or not) on every request. Recall that the Authenticate verb gets the user info, but only if it exists. When the request is run, the authentication middleware asks the default scheme auth handler to run its authentication code

### Additional Resources

* Some information taken from the links provided above

