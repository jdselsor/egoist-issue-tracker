# Egoist Issue Tracker
## Project Goal
The goal of this project is to create an issue tracker system. This system will include a website that allows users to submit issues, allow community managers to aggregate issues and categorize them into issue reports, allow development team leads to assign priorities to the issue reports and also assign teams to issues, lastly this system will allow teams to track progress on the issue reports.
### Subgoals
#### Website
The website will allow anyone to submit an issue to the system. This issue will be logged into a database that is a collection of all submissions that can be viewed by any Community Managers. The Community Managers then will group all the similar reports into an issue report. These issue reports will be able to be viewed on the website. A user will be able to see the issue, date reported, and status.
#### Company Issue Manager Application
This is a C# application that will allow an employee to log in and view relevant information. If they are a community manager they will see the issue’s table. They will be able to view an issue and assign it to an issue report. This report should have a collection of issues and a summary of it as well as all the log files submitted with the issues. The development leads will be able to see all issue reports. Then the lead developers will give issue reports a priority and a team. The lead developer of the team will assign the tasks to team members. Each developer will be able to see all the issues that their team has and all tasks assigned to them. When an issue is assigned to a team each member will get an email and if they opt-in to it they will receive a text as well.
#### Database
The database will be build using PostgreSQL

## Tasklist
- [ ] Website
	- [ ] Create a homepage that lets the user choose to submit an issue or view active issues.
	- [ ] The submit page an issue will be a form that asks the user for an email, description, and a log file. When the user presses the submit button this form is validated and sent to the database.
	- [ ] The view issue page will show all active issue reports. It will show the user the issue priority, issue description, and progress. 
- [ ] Company Application
	- [ ] Create a login setup
		- [ ] When an employee submits the email and password the application will send a query to the database requesting the password associated with the email. Both should be encrypted using the MD5 algorithm and salting the hash. If the login returns true it will allow the employee to view the information and use functions.
	- [ ] Allow a user to view the information relevant to them
		- [ ] A Community Manager will see all issues
		- [ ] A Team Lead will see all issue reports and all tasks assigned to them
		- [ ] A Developer will see all issues assigned to them and all tasks assigned to them
	- [ ] Allow a user to add to tables
		- [ ] A Community Manager will only be able to add to the Issue Report Table.
		- [ ] A Team Lead can add to the Task Table and assign a team member to it and they can accept an Issue Report and give it a priority.
		- [ ] A Developer can on completion of a Task give that task a completed status.
- [ ] Database
	- [x] ~~Create an ER diagram~~ Completed on February 19 2020 at 10:52 am
	- [x] ~~Create a Relational diagram~~ Completed on February 19 2020 at 11:30 am
	- [ ] Create tables in the database
	- [ ] Draft queries
	- [ ] Link database to website and company application
	
# ER Diagram
[Imgur](https://imgur.com/a/ETPYX7b)
