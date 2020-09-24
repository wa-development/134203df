# Index
## A) Installation
## B) What we're looking for
## C) Notes
## D) NB: Submiting Your Results
## E) Test

# A Installation:
1. Download and install Sql Server Express (any edition + 2015)

1.2. Connect to the server:

1.2.1 Ensure Sql Server express service is running.

1.2.2 Connect to the server using SSMS to test (the connection string would be in the Sql Express complete box, use that within your application later

2. Download and install visual studio (2015 +). Ensure the web components are selected for installation.

3. Setup the interview database

3.1 Create a folder in "c:\data".

3.2 Run the file **interview.sql** in the **database** folder, in a SSMS to create the database required for this project.

4. Run the project:

4.1 Open Interview.sln, and make sure to build, run/debug the application, to ensure everything is running smoothly.

4.2 The project should run fine within VS2015, however when using VS2017/vs2019, the application my not build due to a msbuild csc issue between previous versious. Open the project properties > and change the CPU build configuration from default/any to X64 (or X86) > build and run > Revert back to default > Build and Run again. Fix Video: https://recordit.co/9aWuqtfCj2

# B What we're looking for:

- Good object-orientated design, considering concepts like SOLID principles, reusability etc.

- Attempts at good structural, creational and architectural design patterns.

- Concepts promoting high cohesion and loosely coupling like IOC.

- Knowledge of asp.net frameworks and external frameworks, like asp.net controls, forms authentication and ORMS.

- Completing the project is always important.

# C Notes:

- The application is a simple employee and project management application.
- The database should be easy enough to look over and figure out.
- If you're uncertain about a requirement, continue, and explain your approach taken via code comments and/or a followup document/email.

# D Submiting Your Results:

- This is a 4 hour test, and the submission has to be done within the 4 hour time frame. The project should be made available to you with an hour extra to allow to for setting up your envrionment and project.
- Submit the test by either: 1) Emailing the results. 2) Uploading it to a shared folder (Google Drive, DropBox etc) and sharing it with the Webafrica co-ordinator. (We advise you Zip your project)
- The submitted result should include: 1) The entire .net project file. 2) An scripted export your database script.
- This git repository is setup to be read-only, so you won't be to commit back to the repository.

# E Test:
### 1. Add an Employee


- **NB: The application receives input from 2 entry points, a console application and webform, you will have to cater for receiving from both.**


#### 1.1 Add a new column to the dbo.Employee table called DateOfBirth
#### 1.1.1 Alter the web form to capture the date of birth.
#### 1.1.2 Alter the console application to accept a date of birth input.

#### 1.2 Allow the "Add Employee" interfaces (i.e. both the web application and console application), to store an employee to dbo.Employee table.

### 2. View projects</h3>
#### 2.1 On the View projects page, read the projects from the dbo.Project table, displaying them in the list view.
#### 2.2 The Employees column is comma seperated list of all employees who has worked on those projects. Display these as well, and ensure the projects without employees also gets viewed.

### 3. Business Calculation </h3>

#### Business has added a new rule. It states that, each Employee, depending on their Job Title, would add an additional cost to the Project they're part of:
#### a) Developer: 2500
#### b) DBA: 3000
#### c) Tester: 1000
#### d) Business Analyst: 4500

#### 3.1 Calculate the cost of each of the projects, **including the new business rule** costs. Display the result in the ViewProjects.aspx, "cost" column.
