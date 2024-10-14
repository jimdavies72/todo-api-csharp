# todo-api-csharp

- C# REST API Tutorial - can be found here:
  - [MS REST API Tutorial](https://learn.microsoft.com/en-us/aspnet/core/tutorials/first-web-api?view=aspnetcore-8.0&tabs=visual-studio-code)

## List of C# terminal commands

- Create a new web API project :

  - `dotnet new webapi --use-controllers -o TodoApi`

- Add a nuget package:

  - `dotnet add package Microsoft.EntityFrameworkCore.InMemory`

- Trus dotnet certs\*:

  - `dotnet dev-certs https --trust`
  - This didnt work in my environment, Chrome still blocked the server:port. Therfore to combat this I typed at the blocked page:
    - `thisiunsafe`

- Run the app:

  - `dotnet run --launch-profile https`
  - add` /swagger `to the uri to run swagger app

- Scaffold the TodoItemsController:

  - `dotnet aspnet-codegenerator controller -name TodoItemsController -async -api -m TodoItem -dc TodoContext -outDir Controllers`
