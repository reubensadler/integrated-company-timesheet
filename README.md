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


