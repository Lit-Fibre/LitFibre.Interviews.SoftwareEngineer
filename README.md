# Lit Fibre Software Engineer C# Exercise

### You'll need
Visual Studio 2022 w/ .NET 6.

Optionally:
Curl/Postman/Insomnia - the project includes the Swagger frontend so not strictly necessary.

## The exercise
### Task 1
Implement the `IMemoryDatabase` interface for the `Order` model. As the interface name implies, this should be a simple in-memory DB, likely implemented using just a List or a Dictionary. We've provided some seed data in `orders.json` that you can use to initialize the DB if you wish.

### Task 2
Implement a number of RESTful endpoints that interact with your order database. The endpoints should be the following:
1. Read all orders.
2. Read an order by ID.
3. Add an order.
4. Delete an order.
5. Update an order.
6. Read all orders that contain a specified product code.
7. Read all orders that were placed after a specified date.

You can create these using MVC actions in the `LitFibre.Interviews.SoftwareEngineer.Controllers.OrderController` API controller, or you can use [Minimal APIs](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/minimal-apis?view=aspnetcore-6.0) in `Program.cs`.

You don't need to create a frontend to consume these endpoints, we will test them with Swagger/Postman.

### If you finish early
Feel free to expand on the API, database and models if you feel it will help demonstrate your knowledge of C#, data structures, web APIs, dependency injection, or whatever you'd like to show off. This is entirely optional.

### Guidelines
1. Try and keep your work confined to the three projects we've provided in the solution. Best practices may dictate that there should be more separation but for the sake of the exercise, we'd like to keep it simple.
	- The main project should contain the startup code, any configuration and dependency injection, and your REST endpoints.
	- The `Models` project contains basic classes to be used with the database.
	- The `Services` project should contain any "business logic", including your implementation of `IMemoryDatabase`.
2. Complete as much of the exercise as you can, as well as you can, within the assigned timeframe, but don't worry if you feel at the end that you could have done more. We're happy to discuss your ideas with you afterwards.

### GLHF!
