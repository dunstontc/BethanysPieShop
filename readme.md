# ASP.NET Core 2.0 MVC

## ASP.NET Core 2.0
- ASP.NET Core 2.0 is build on .NET Core
- Not tied to .NET framework

## MVC
- Architectural pattern
- Separation of concerns
- Promotes testability & maintainibility

## Structure
- Dependency Injection for our own services. Create more loosely coupled code.

### `Startup` class
- By default, the `Startup` Class contains two methods: `ConfigureServices()` & `Configure()`
- Both methods are automatically called by ASP.NET Core.
- In the *ConfigureServives* method we will add services to the dependency injection container.  
- Through the passed-in IServiceCollection we are capable of registering services in our ASP.NET Core application. 

### Model
- The group of classes that make up the domain data (and the logic to manage that data.)
- Should ideally have a simple API.
- Hides detalis of managing the data from the user.

- Repository Class
  - Allows our code to use objects without knowing how they are persisted.

## Controllers
- Inherit from the base Controller class
- Name will be suffixed with *Controller*
- Responds to incoming requests
- *Constructor Injection*

## Terms
- POCO - Plain old clr classes
