# ordersystem

## Usage
* Set OrderSystem.API as  a startup project
* Run the project,this will open https://localhost:<port>/swagger/index.html,
* For Tests,  run  the following command in PowerShell 
```bash
dotnet test
```
## Approach
* used Monolithic Clean Architecture approach, to eliminate  a  dependency nightmare, simplifies  deployment,t and
Manage  all code in a single codebase to reduce  complexity

## Missing Technical Features
* CQRS with MediatR
* Repository Pattern( with unitOfwork)
* Cashing Strategy(Redis  etc)
* APi Versioning.
* Entity Framework Core (EF Core) for data access
* AutoMapper for object mapping
* FluentValidation for input validation
* Serilog for logging.
* Secure authentication and authorization with ASP.NET Identity + JWT 

## Assumptions
* Hardcoded Discount percentages  for customer strategies should be generic  anyway(configurable from UI  settings)
* Using in-memory data(should  connect to a persistent storage).
