# Eau Claire's Salon

#### By Matt Wilkinson

#### A simple MVC web application to help Eau manage her employees (stylists) and their clients.

## Github links

https://github.com/wilkinsonmatt/Salon.git

## Technologies Used

* C#
* Net 5.0
* Markdown
* CSS
* MySQL WorkBench
* EntityFrameWork
* HTML


## Description

A C# program that allows Eau be able to add a list of stylists working at the salon, and for each stylist, add clients who see that stylist. The stylists have specific specialties, so each client can only see (belong to) a single stylist.

## Setup/Installation Requirements

* Download/Clone entire github file
* Open root directory with Bash
* cd into HairPlace/HairSalon
* Create an appsetting.json file at the root directory_*
* Open the appsetting.json file and enter:
```
{ 
  "ConnectionStrings": { 
    "DefaultConnection": "Server=localhost;Port=3306;database=[Database-Name];uid=root;pwd=[Your-Password;" 
  } 
}
```
* Open MySQL WorkBench 
* In the Navigator > Administration window, select Data Import/Restore
* In Import Options select Import from Self-Contained File
* You will use .sql file type that is located the root directory ```HairSalon.Solution```.
* Navigate to the tab called Import Progress and click Start Import at the bottom right corner of the window.
* After you are finished with the above steps, reopen the Navigator > Schemas tab. Right click and select Refresh All.
* Import the database named "matt_wilkinson.sql" from the root directory of the project.<br><br>
How to import the database:
  <li>Open SQL Workbench.
  <li>Navigate to "Administration" tab in SQL Workbench.
  <li>Click "Data Import/Restore".
  <li>Select the radio button "Import from Self-Contained File" and include file path to the sql file of this project you cloned to your machine.
  <li>In "Default Schema to be Imported to" click "New".
  <li>Name the schema "matt_wilkinson" then click "OK".
  <li>Once named, switch to "Import Progress" tab and click "Start Import

<br>
- run ```dotnet restore``` and ```dotnet build``` then ```dotnet run```

- click on  <http://localhost:5000>

## Known Bugs

* not able to list clients in sytlist details, but able to list stylist next to client in client index

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