Project Setup Instructions

IDE: Visual Studio

Framework: .NET 6.0

User Interface: Swagger

Authentication: JWT

Libraries Used:

MediatR 12.2.0
MediatR.Extensions.Microsoft.DependencyInjection 11.1.0
Microsoft.AspNetCore.Authentication.JwtBearer 6.0.28
Microsoft.EntityFrameworkCore 6.0.28
Microsoft.EntityFrameworkCore.Design 6.0.28
Microsoft.EntityFrameworkCore.SqlServer 6.0.28
Microsoft.EntityFrameworkCore.Tools 6.0.28
Swashbuckle.AspNetCore 6.2.3

Setup Instructions:

Clone the Project from GitHub:

Clone the project repository from GitHub using Git command or any Git client.
Open Project in Visual Studio:

Launch Visual Studio.
Open Solution:

Open Visual Studio.
Select "Open a project or solution" from the start window or navigate to "File" > "Open" > "Project/Solution".
Browse to the directory where you extracted the project and open the solution file (.sln).
Restore NuGet Packages:

Restore NuGet packages for the solution to ensure all dependencies are resolved.
Right-click on the solution in Solution Explorer.
Select "Restore NuGet Packages".
Set up Database:

Configure your local SQL Server instance.
Update the connection string in appsettings.json or appsettings.Development.json to point to your local database.
Run Migrations:

Execute Entity Framework Core migrations to create/update the database schema.
sql
Copy code
add-migration init
Update-Database

Configure JWT Authentication:

Update JWT authentication settings in appsettings.json.
Build and Run:

Build the solution.
Run the application.
Access Swagger UI:

Once the application is running, navigate to the Swagger UI endpoint to interact with the APIs.
bash
Copy code
https://localhost:7015/swagger/index.html

Additional Notes:

Ensure that your local environment meets the prerequisites for running .NET 6.0 applications and SQL Server.
Customize authentication, authorization, and other configurations as needed for your specific use case.
