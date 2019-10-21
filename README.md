
# _Eau Claire's Salon_

#### _A program created to practice the MVC model in ASP.NET using MySQL 10/20/2019_

#### By _Zach Krogh_

## Description

_This web application allows the user to create stylists and then, within those stylists, create lists of clients._

## Setup/Installation Requirements
* _Setup MySQL database as folows:_
  * CREATE SCHEMA \`zach_krogh\`;
  * USE zach_krogh;
  * CREATE TABLE \`stylists\` ( \`stylistid\` serial, \`name\` varchar(255) NULL, \`specialty\` varchar(255) NULL, PRIMARY KEY (\`stylistid\`));
  * CREATE TABLE \`clients\` ( \`clientid\` serial, \`name\` VARCHAR(255) NULL, \`stylistid\` INT(11) NULL, PRIMARY KEY (\`clientid\`));
  * CREATE TABLE  \`stylistclient\` ( \`stylistclientid\` serial, \`clientid\` INT(11) NULL, \`stylistid\` INT(11) NULL, PRIMARY KEY (\`stylistclientid\`));
* _Install dotnet core._
* _Download all files into the same directory and run "dotnet run"_

## Project Specifications

* _The user can create a stylist._
  * _input: name:"Bob" specialty:"hair dye"_
  * _output: none (both are saved to variables)_
  * _description: This is the most basic requirement of the program, allowing the user to create a stylist._
* _The user can create a Client within a stylist._
  * _input: name: "Fred" stylist: "Bob"_
  * _output: none (everything saved to variables)_
  * _description: The next simplest behavior, the user can create a client within a stylist._
* _The user can view details of a client._
  * _input: Navigate to a client._
  * _output: The client details are displayed._
  * _description: Ensure the user can view client details._

## Support and contact details

_contact: zakrogh@gmail.com_

## Technologies Used

_C#, ASP.NET MVC, Razor, HTML, CSS, Bootstrap, MySQL_

### License

*MIT License*

Copyright (c) 2019 **_Zach Krogh_**
