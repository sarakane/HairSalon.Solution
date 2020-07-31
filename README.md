# _Eau Claire's Salon_

#### _C# ASP .NET Core MVC project for Epicodus, 07.31.2020_

#### By _**Sara Kane**_


## Description

MVC web application to help a hair salon owner manage her employees and their clients. 


## Specifications

| User Stories                                                                                                                                         | Input                                              | Output                                      | Completed? |
|------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------|---------------------------------------------|------------|
| As the salon owner, I need to be able to see a list of all stylists.                                                                                 | Click on show all stylists                         | All stylists are shown                      | Y          |
| As the salon owner, I need to be able to select a stylist, see their details, and see a list of all clients that belong to that stylist.             | Click on a stylist                                 | Stylist details are shown                   | Y          |
| As the salon owner, I need to add new stylists to our system when they are hired.                                                                    | Click on add new stylist, fill out stylist details | New stylist is added                        | Y          |
| As the salon owner, I need to be able to add new clients to a specific stylist. I should not be able to add a client if no stylists have been added. | Select a stylist and add a client to that stylist  | Client is assigned to the specified stylist | Y          |




## Setup/Installation Requirements
### Required Software
* [.NET Core 2.2](https://dotnet.microsoft.com/download/dotnet-core/2.2)
* [MySQL Community Server and MySQL Workbench](https://dev.mysql.com/downloads/)

* Clone the GitHub repository by running `git clone https://github.com/sarakane/HairSalon.Solution.git` in the terminal.
  * Or download the ZIP file by clicking on `Code` then `Download ZIP` from this repository.

#### View locally 
* Navigate to the newly created `HairSalon.Solution` folder.
* Navigate to the `HairSalon` project folder.
* In the terminal, run `dotnet restore` and `dotnet build` to build the app and `dotnet run` to run it.
  * Note: you will have to first set up a database. See instructions below.
* Click on the _now lisetning on_ link to open in your browser.

### Database Setup
#### Option 1 - MySql Workbench
* In the Navigator > Administration window, select Data Import/Restore.
* In Import Options select Import from Self-Contained File.
* Select the `sara_kane.sql` file included in this repository.
* Under Default Schema to be Imported To, select the New button.
  * Enter `sara_kane` as the name of the schema.
  * Click Ok.
* Click Start Import.
* Reopen the Navigator > Schemas tab. 
* Right click and select Refresh All and the new database will appear.

#### Option 2 - From the command line 

* Run MySQL by entering `mysql -uroot -p{your password}` in the terminal
* Enter the following commands to create the necessary database and tables:
```
DROP DATABASE IF EXISTS `sara_kane`;
CREATE DATABASE `sara_kane`;

USE `sara_kane`;

DROP TABLE IF EXISTS `clients`;
CREATE TABLE `clients` (
  `ClientId` int NOT NULL AUTO_INCREMENT,
  `ClientName` varchar(255) DEFAULT NULL,
  `ClientPhoneNumber` varchar(255) DEFAULT NULL,
  `StylistId` int NOT NULL DEFAULT '0',
  PRIMARY KEY (`ClientId`)
);

DROP TABLE IF EXISTS `stylists`;
CREATE TABLE `stylists` (
  `StylistId` int NOT NULL AUTO_INCREMENT,
  `StylistName` varchar(255) DEFAULT NULL,
  PRIMARY KEY (`StylistId`)
);
```
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