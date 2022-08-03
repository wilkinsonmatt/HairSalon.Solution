# Eau Claire's Salon

#### By Matt Wilkinson

#### A simple MVC web application to help Eau manage her employees (stylists) and their clients.

## Github links

https://github.com/wilkinsonmatt/HairSalon.Solution.git

## Technologies Used

* C#
* Net 5.0
* Markdown
* CSS
* MySQL WorkBench
* EntityFrameWork
* HTML


## Description

A C# program that allows Eau to be able to add a list of stylists working at the salon, and for each stylist, add clients who see that stylist. The stylists have specific specialties, so each client can only see (belong to) a single stylist.

## Setup/Installation Requirements

* Download/Clone entire github file
* Open root directory with Bash
* cd into HairSalon.Solution/HairSalon
* Create an appsetting.json file at the root directory
* Open the appsetting.json file and enter:
```
{ 
  "ConnectionStrings": { 
    "DefaultConnection": "Server=localhost;Port=3306;database=matt_wilkinson;uid=root;pwd=[YOUR PASSWORD];" 
  } 
}
```
* Import the database named "matt_wilkinson.sql" from the root directory of the project into MySQL.<br><br>
How to import the database with MySQL:
* Open SQL Workbench.
* Click the "Administration" tab on the left side of the page
* Click "Data Import/Restore" 
* Select "Import from Self-Contained File" and change the file location to "matt_wilkinson.sql"
* Then click the "New" button next to the "default Target Schema"
* Name the schema "matt_wilkinson"
* Click "ok"
* Click "Start import" at the bottom of the page
<br>
* Run the following commands in the command line:
  <br>1: dotnet restore
  <br>2: dotnet build
  <br>3: dotnet run
* click on  <http://localhost:5000>

## Known Bugs

* not able to list clients in sytlist details, but able to list stylist next to client in the client index

## License

Copyright (c) 2022 Matt Wilkinson

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR I