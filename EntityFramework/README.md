# EntityFramework
##

### How Entity Framework Migrations Work:
- Enable migrations
- Create migrations

**Migration format**: YYYYMMDDHHSST_Name
  

### the sequence of steps:
* Add EntityFramework (now 6.1.3) NuGet package.
* Switch to the Package Manager Console (PowerShell console right within Visual Studio)
* Select Default Project
* Setup startup project. That's going to be important because the .config inside of project is where we'll get our connection string.
* Create DbContext : class MyContext:DbContext
* PM> Enable-Migrations *(This creates a Migrations folder, and initializes it with a configuration class. One important thing here is that AutomaticMigrationsEnabled is set to false)*
* Pass the connections string name into the DbContext constructor (like, :base(connectionString)) `<add connectionString=""/>`
* PM> Update-Database
* PM> Add-Migration NameMigration

**change model:**
```cs
protected override OnModelCreating(DbModelBuilder modelBuilder) 
{
	modelBuilder.convetions.Remove<PluralizeingTableNameConvention>();
	base.OnModelCreating(modelBuilder);
}
```



### Resuources:
* Michael L Perry, Architect and team lead at improving @michaellperry and [qedcode.com](http://qedcode.com)
* [thedatafarm.com](http://thedatafarm.com) by JulieLerman
* [Code First Migrations in Team Environments. Rowan Miller. MSDN.](https://msdn.microsoft.com/ru-ru/data/dn481501)
* EF7 Migrations: Not New, but Definitely Improved. Julie Lerman. The Data Farm.
* Entity Framework Code First Migrations. Julie Lerman. Pluralsight.
