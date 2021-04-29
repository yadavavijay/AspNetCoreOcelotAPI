# AspNetCoreOcelotAPI
Implement API Gateways with Ocelot
Need of API Gateway:
	1. Traffic Routing
	2. Exposed Unified End Points
	3. API Composition
	4. Caching
	5. Logging
	6. Authentication
	7. Authorization
	8. Load Balancing
	9. Service Discovery

Development Setup Required:
	1.  Visual Studio 2019
	2.  SQL Server 2017 Express Edition
	3. .NET Core 3.1
	
NuGet Packages required:
	microsoft.entityframeworkcore
		Entity Framework Core is a modern object-database mapper for .NET. It supports LINQ queries, change tracking, updates, and schema migrations. EF Core works with SQL Server, Azure SQL Database, SQLite, Azure Cosmos DB, MySQL, PostgreSQL, and other databases through a provider plugin API.
	microsoft.entityframeworkcore.sqlserver
	Microsoft.EntityFrameworkCore.Tools
		Enables these commonly used commands:
		Add-Migration
		Drop-Database
		Get-DbContext
		Get-Migration
		Remove-Migration
		Scaffold-DbContext
		Script-Migration
		Update-Database

Open SQL Server Database :
	Create a new Database named as UserMicorservice
Add SQL Server Database connection string to .NETCore application

Package Manager Console Host Version 5.7.0.6726

Type 'get-help NuGet' to see all available NuGet commands.

PM> add-migration initial
Build started...
Build succeeded.
To undo this action, use Remove-Migration.
PM> update-database -verbose
Using project 'UserService'.
Using startup project 'UserService'.
Build started...
Build succeeded.
 
http://localhost:56674/api/user

Use Postman also.

Ocelot API Gateway :
	• An Open-Source API Gateway For .NET Platform
	• Lightweight and run on platform that supports ASP.NET Core
	• Provides all the necessary features of an API Gateway
	• Used by Microsoft itself for their projects

Integrating Ocelot API Gateway:
	Add new project as ASP.NET core web application with empty project
