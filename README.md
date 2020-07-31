# _Eau Claire's Salon_

#### _C# ASP .NET Core MVC project for Epicodus, 07.31.2020_

#### By _**Sara Kane**_


## Description

MVC web application to help a hair salon owner manage her employees and their clients. 


## Specifications

| User Stories                                                                                                                                         | Input                                              | Output                                      | Completed? |
|------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------|---------------------------------------------|------------|
| As the salon owner, I need to be able to see a list of all stylists.                                                                                 | Click on show all stylists                         | All stylists are shown                      | N          |
| As the salon owner, I need to be able to select a stylist, see their details, and see a list of all clients that belong to that stylist.             | Click on a stylist                                 | Stylist details are shown                   | N          |
| As the salon owner, I need to add new stylists to our system when they are hired.                                                                    | Click on add new stylist, fill out stylist details | New stylist is added                        | N          |
| As the salon owner, I need to be able to add new clients to a specific stylist. I should not be able to add a client if no stylists have been added. | Select a stylist and add a client to that stylist  | Client is assigned to the specified stylist | N          |




## Setup/Installation Requirements
#### Required Software
* [.NET Core 2.2](https://dotnet.microsoft.com/download/dotnet-core/2.2)
* [MySQL Community Server and MySQL Workbench](https://dev.mysql.com/downloads/)

* Run MySQL by entering `mysql -uroot -pepicodus` in the terminal
* Enter the following commands to create the necessary database and tables:
```
DROP DATABASE IF EXISTS `sara_kane`;
CREATE DATABASE `sara_kane`;
USE DATABASE `sara_kane`;

```
* Clone the GitHub repository by running `git clone https://github.com/sarakane/HairSalon.Solution.git` in the terminal
* Navigate to the newly created `HairSalon.Solution` folder
* Navigate to the `HairSalon` project folder and run `dotnet restore`
* Run `dotnet build` to build the app and `dotnet run` to run it
* Click on the _now lisetning on_ link to open in your browser 


## Known Bugs

* No known bugs.
 


## Technologies Used

* C# 
* .NET Core 2.2
* ASP.NET Core MVC
* MySQL Server 8.0.21
* Visual Studio Code
* Git
* GitHub


### License

*This site is licensed under the MIT license.*

Copyright (c) 2020 **_Sara Kane_**