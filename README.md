# Index
## A) Installation
## B) NB: Requirements & Constraints
## C) What we're looking for
## D) Notes
## E) NB: Submiting Your Results
## F) Test

# A Installation:
1. Download and install Sql Server Express (any edition + 2015)

1.2. Connect to the server:

1.2.1 Ensure Sql Server express service is running.

1.2.2 Connect to the server using SSMS to test (the connection string would be in the Sql Express complete box, use that within your application later

2. Download and install visual studio (2015 +). Ensure the web components are selected for installation.

3. Setup the interview database

3.1 Create a folder in "c:\data".

3.2 Run the file **interview.sql** in the **database** folder, in a SSMS to create the database required for this project.

# B Requirments & Constraints

The application is a simple employee and project management application. The database has primary and foreign key column represented in the tables, to reflect the relationship between different entities in the system.

You are required to build a website/web application, that allows a user to add an employee to the database. 
You are required to build a web page/view, to show the various projects in the database.

### The front-end for the project MUST BE created using one or a combination of the below technologies/programming languages:
- HTML / CSS / SASS / LESS / JAVASCRIPT
- Asp.Net or Asp.Net Core
- Mvc (core or full framework)
- ReactJS

### The back-end for the project MUST USE:
- C# (full framework or core)

# C What we're looking for:

- Good object-orientated design, considering concepts like SOLID principles, reusability etc.

- Attempts at good structural, creational and architectural design patterns.

- Concepts promoting high cohesion and loosely coupling like IOC.

- Knowledge of using nuget packages / nodejs libraries where applicable.

- Completing the project is always important.

# D Notes:

- The application is a simple employee and project management application.
- The database should be easy enough to review and understand.
- If you're uncertain about a requirement, continue, and explain your approach taken via code comments and/or a followup document/email.

# E Submiting Your Results:

- This is a 8 hour test, and the submission has to be done within the 8 hour time frame. The project should be made available to you with an hour extra to allow to for setting up your envrionment and project.
- Submit the test by either: 1) Emailing the results. 2) Uploading it to a shared folder (Google Drive, DropBox etc) and sharing it with the Webafrica co-ordinator. (We advise you Zip your project)
- The submitted result should include: 1) The entire .net project file. 2) An scripted export your database script.
- This git repository is setup to be read-only, so you won't be to commit back to the repository.

# F Test:
### 1. Add an Employee

#### 1.1 Add a new column to the dbo.Employee table called DateOfBirth

#### 1.1.1 Create a console application, that accepts inputs for adding an employee, and store the data in the "Employee" table.

#### 1.1.2 Create a web page (/addemploy.html | .aspx | etc) that accepts inputs for adding an employee, and store the data in the "Employee" table.

### 2. View projects</h3>

#### 2.1 Create a web page to view projects (/viewprojects.html | .aspx | etc), that shows the following columns:

|Project Name|Start Date|End Date|Employees|Cost|

- Project Name: This should simply be the name of the project
- Start Date: Start date of the project
- End Date: End date of the project
- Employees: A comma-seperated list of the employees First name and Surnames that was involved in the project.
- Cost: Cost of the project

#### 2.2 Note: Be sure to include projects that also do not have any employees.

### 3. Business Calculation </h3>

#### Business has added a new rule. It states that, each Employee, depending on their Job Title, would add an additional cost to the Project they're part of:
#### a) Developer: 2500
#### b) DBA: 3000
#### c) Tester: 1000
#### d) Business Analyst: 4500

#### 3.1 Calculate the cost of each of the projects, **including the new business rule** costs. Display the result in the viewprojects, "cost" column.
