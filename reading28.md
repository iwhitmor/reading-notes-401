# Auth & Cookies

## [HTTP Cookies](https://developer.mozilla.org/en-US/docs/Web/HTTP/Cookies)

* An HTTP cookie (web cookie, browser cookie) is a small piece of data that a server sends to a user's web browser

* Typically, an HTTP cookie is used to tell if two requests come from the same browser—keeping a user logged in, for example

* Cookies are used for three things:

  * Session Management

    * Logins, shopping carts, game scores, or anything else the server should remember

  * Personalization

    * Logins, shopping carts, game scores, or anything else the server should remember

  * Tracking

    * Recording and analyzing user behavior

* Lifetime of a cookie can be defined in two ways:

  * Session Cookies

    * Deleted when the current session ends. The browser defines when the "current session" ends, and some browsers use session restoring when restarting. This can cause session cookies to last indefinitely

  * Permanent Cookies

    * Deleted at a date specified by the Expires attribute, or after a period of time specified by the Max-Age attribute

## [HTTP Cookies Explained](https://humanwhocodes.com/blog/2009/05/05/http-cookies-explained/)

* What is a COOKIE?

  * A small text file that is stored by a browser on the user’s machine. Cookies are plain text; they contain no executable code. A web page or server instructs a browser to store this information and then send it back with each subsequent request based on a set of rules. Web servers can then use this information to identify individual users

* Why might a COOKIE be automatically removed from the browser?

  * Session cookies are removed when the session is over (browser is closed)

  * Persistent cookies are removed when the expiration date and time have been reached

  * If the browser’s cookie limit is reached, then cookies will be removed to make room for the most recently created cookie. For more details, see my post on cookie restrictions.

* The COOKIE technique created more than ten years ago is still in use in almost the exact same way as it was first implemented

## [.NET Cookies Simplified](https://asp.mvc-tutorial.com/httpcontext/cookies/)

* Pretty much all server-side technologies have built-in support for handling cookies and of course the ASP.NET MVC framework does as well

* Cookies all you to be able to save information about the visitor and retrieve it again on subsequent requests. This is a very important technique, used in a wide range of situations, like keeping the user logged in, tracking their use of your website and much more

### Additional Resources

* Some information taken from the links provied above
