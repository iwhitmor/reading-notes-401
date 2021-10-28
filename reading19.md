# Roles, Claims, Tokens

## [Claims-Based Auth](https://docs.microsoft.com/en-us/aspnet/core/security/authorization/claims?view=aspnetcore-2.1)

* A claim is a name value pair that represents what the subject is, not what the subject can do

* Claims based authorization, at its simplest, checks the value of a claim and allows access to a resource based upon that value

* An identity can contain multiple claims with multiple values and can contain multiple claims of the same type

* Claim based authorization checks are declarative - the developer embeds them within their code, against a controller or an action within a controller, specifying claims which the current user must possess, and optionally the value the claim must hold to access the requested resource. Claims requirements are policy based, the developer must build and register a policy expressing the claims requirements

## [Intro To Claims](https://andrewlock.net/introduction-to-authentication-with-asp-net-core/)

* Authentication

  * The process of determining WHO you are

* Authorisation

  * What you are ALLOWED to do

* Claims Based Authentication

  * A statement about, or a property of, a particular identity which contains a name and a value

    * E.G. Name, Date of birth, Email, etc

  * The identity itself represents a single declaration that may have many claims associated with it

* Multiple Identities

  * It is possible to have multiple forms of identification. Think a passport and an ID, or a piece of mail specific to your household, or a specific email and password

  * The key points here are that a principal can have multiple identities, these identities can have multiple claims, and the ClaimsPrincipal inherits all the claims of its Identities

## [JWT Authentication](https://codeburst.io/jwt-to-authenticate-servers-apis-c6e179aa8c4e)

* JSON Web Token

  * In simple terms, it is just another way of encoding JSON object and use that encoded object as access tokens for authentication from the server

  * There are 3 parts to the JWT

    * Header

    * Payload

    * Signature

* Two parties involved

  * Producer

    * The one who gives a service. It will be the provider(Server) of the API(s) which are JWT protected

  * Consumer

    * The one who uses it. It will be the customer(Server/Mobile App/ Web App/ Client) who will be providing the valid JWT token to consume the API(s) being provided by the Producer

### Additional Resources

* Some information taken from the links provided above
