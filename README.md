# _Building an API_
## Cretaceous Park
### An independent project for Epicodus

#### _A program that creates an API of state and national parks in the United States._

#### By Brent Hubbard

## Technologies Used

* _C#_
* _.NET 5.0.102_
* _<span>ASP.NET</span> Core Mvc 4.8_
* _Swagger_
* _MySQL_
* _Razor_
* _Entity Framework Core_
* _Git_

## Description

_This application creates a database to hold parks and their respective sizes and locations. One can create, update, or delete parks. One can also see a list of all parks. One can ALSO pick a random park from the data to check out._

## Setup/Installation Requirements

* You can clone the repository to your desktop
* Navigate to the ParksApi directory
* Add a file called appsettings.json. In that file, you will need to add the following code:
<pre>
{
  "Logging": {
    "LogLevel": {
      "Default": "Information",
      "Microsoft": "Warning",
      "Microsoft.Hosting.Lifetime": "Information"
    }
  },
  "AllowedHosts": "*",
  "ConnectionStrings": {
    "DefaultConnection": "Server=localhost;Port=3306;database=park;uid=root;pwd=<em>password</em>;"
  }
}
</pre>
* The 'password' is only necessary if you have a password for your MySQL
* Save
### Setting up the database
#### Using SQL
1. Open a SQL command line in a terminal. Copy and paste the contents of brent_hubbard.sql and hit enter.
2. Quit out of SQL with Ctrl + c
#### OR Using Entity Framework Core
1. In the terminal, navigate to the ParksApi directory
2. Enter "dotnet ef database update"
### Running the program
* From the ParksApi directory, enter "dotnet restore"
* Next, enter "dotnet build"
* Enter "dotnet run" in the terminal and hit enter to start a local host. 
* Ctrl + click the link that populates in the terminal to view the application in the webpage. It is probably http://localhost:5000/
* Use Ctrl + C in the terminal to quit the host and close out of the window in the browser.
### Checking the API documentation using Swagger
* Whatever URL your local host is using, just add "/swagger" to the end of it!
* You can also USE the API from here. Just click one of GET, POST, PUT, or DELETE buttons, and then click Try it out. 

## Known Bugs
 _No known bugs. _
## License

[MIT](https://opensource.org/licenses/MIT)

Copyright ?? 2021 Brent Hubbard

All Rights Reserved

## Contact Information
Hubbardbrent@hotmail.com
