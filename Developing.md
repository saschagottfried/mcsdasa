# Developing Microsoft Azure Solutions


## Patterns
- Head First Design Patterns
- [doFactory Patterns Framework](http://dofactory.com/products/sql-database-design-pattern-framework)
  - .NET
  - Javascript
  - SQL

## Web Apps

ASP.NET MVC

- Routes
- Controller
- Views
- Global.asax

## Storage Emulator
- https://docs.microsoft.com/en-us/azure/storage/storage-use-emulator


## Azure WebJobs
- [Get Started](https://docs.microsoft.com/en-us/azure/app-service-web/websites-dotnet-webjobs-sdk-get-started)
- [WebJobs SDK](https://docs.microsoft.com/en-us/azure/app-service-web/websites-dotnet-webjobs-sdk)
- [Running Locally](https://github.com/Azure/azure-webjobs-sdk/wiki/Running-Locally#development-settings)
- [WebJobs SDK Extensions](https://github.com/Azure/azure-webjobs-sdk-extensions)
- [Documentation resources](https://docs.microsoft.com/en-us/azure/app-service-web/websites-webjobs-resources)


# Azure SQL
- Database as a service

Security
- add firewall rule for access from specific IP addresses

Geo-Replication
- available in all tiers
- if replicas are readable we call this "Active Geo-Replication"
- You can use the replica of the database as a read-only data source in load-balancing scenarios
  - Example: An application uses the primary database for line-of-business functionality and the replica for reports


# Entity Framework

## Conventions

Primary key convention
- identifier have name: {Id} oder {classname}Id

Custom primary key convention
- ModelBuilder Fluent API

Loading related data
- [lazy loading](https://msdn.microsoft.com/en-us/library/jj574232(v=vs.113).aspx#Lazy Loading)
  - do not do this in WebApi projects - JSON serializer will trigger lazy loading)
- [eager loading](https://msdn.microsoft.com/en-us/library/jj574232(v=vs.113).aspx#Eagerly Loading)
- [explicit loading](https://msdn.microsoft.com/en-us/library/jj574232(v=vs.113).aspx#Explicitly Loading)


Connection String conventions

    public class EventsContext : DbContext
    {}

    <connectionStrings>
    <add name="EventsContext" connectionString="Data Source=(LocalDb)\MSSQLLocalDB;Initial    Catalog=EventsContextModule3Demo;Pooling=True;Integrated Security=True" providerName="System.Data.SqlClient" />
    </connectionStrings>


Database Initializers
- CreateIfDatabaseNotExits
- DropCreateDatabaseAlways
- DropCreateDatabaseIfModelChanges
- MigrateDatabaseToLatestVersion


