# Integrated company timesheet
A group of connected Excel workbooks that lets an employer view hours worked each week both per employee and per project, produced for my employer.
Each employee has their own workbook, and each week their hours worked are transferred to the company timesheet at the push of a button.

### Note that you must have all three workbooks (Company timesheet, Jobs list and Employee timesheet) open for everything to function correctly. 
This was not the case as originally designed, but I made some changes to allow anyone downloading from the repo to test it without needing to change filepaths.
The version used by my employer opens the workbooks automatically when needed.

Feature overview:
* Designed to work using a file sharing service such as Dropbox
* New projects in the added to the company timesheet are automatically added to employee timesheets
* Most functions (such as adding a new employee or project to the company timesheet) are automated, making them much quicker and allowing for input validation
* Only those with access to the company timesheet are able to confirm a weekly timesheet and transfer it, or see timesheet information for other employees

### Instructions
#### Employee timesheet

When a new person joins the company, first create an timesheet for them, entering their full name into the details sheet. Then share with them their timesheet and the jobs list. In the company timesheet, go to the New employee sheet and click Create new employee sheet. Enter their name exactly as entered into their timesheet, and they're good to go.

<img src="Screenshots/Create%20new%20employee%20sheet.png" width="500" >

Each week, the employee should go onto the "blank" worksheet and click Copy sheet. This automatically creates the weeks timesheet with the correct week number and date.

<img src="Screenshots/Copy%20blank%20weekly%20timesheet.png" width="500" >

They can then fill in the hours worked on each project as they go, entering the project name in column A and the start and finish times in column D.

At the end of the week the employer checks the timesheet for each employee and if they're happy, clicks Confirm timesheet. This collects all the information from that week and copies it into the employee's sheet in the company timesheet.

<img src="Screenshots/confirm%20weekly%20timesheet.png" width="500" >

The hours worked on each project by an employee can be view on their sheet in Company timesheets.

<img src="Screenshots/Employee%20summary.png" width="500" >

The Project hours sheet lets the employer see the total hours worked on each project by all employees, broken down by employee.

<img src="Screenshots/Job%20summary.png" width="500" >

To add a new project to all timesheets, simply click the corresponding button in the Projects sheet. Enter the name of the project in the message box (if nothing is entered, or the name already exists, the user will be prompted to enter a valid name). If it is a standard project or a non-chargeable project, a project number will automatically be added. Enter the client and contact name if desired. Projects can also be deleted; clicking the button prompts the user to enter the name of the project to delete. This removes the project from all timesheets.

<img src="Screenshots/add%20and%20delete%20projects%20from%20list.png" width="500" >

When adding or deleting projects, the change is made in both the company timesheet and Jobs list.xlsx. Employee timesheets then refer to Jobs list.xlsx to get the list. This allows the jobs list to easily be shared with all employees without giving them access to the company timesheet.
