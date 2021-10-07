# Expense Reimbursement System

## Project Description

The Expense Reimbursement System (ERS) will manage the process of reimbursing employees for expenses incurred while on company time. All employees in the company can log in and submit requests for reimbursements and view their past tickets and pending requests. Managers can log in and view all reimbursement requests and past history for all employees in the company. Managers are authorized to approve and deny requests for expense reimbursements.

## Technologies Used

* Tech 1 - JavaScript, HTML, CSS, SQL, Postman, AWS RDS, Java, Javalin, Hibernate
* Tech 2 - HTML
* Tech 3 - CSS
* Tech 4 - SQL
* Tech 5 - Postman
* Tech 6 - AWS RDS
* Tech 7 - Java
* Tech 8 - Javalin
* Tech 9 - Hibernate
* Tech 10 - Maven



## Features

List of features ready and TODOs for future development
* Submit Reimbursements
* Retrieve Reimbursements
* Accept/Decline Reimbursements

To-do list:
* Include Angular/Spring
* Imporve UI

## Getting Started
   
git clone https://github.com/Cwall0623/Expense-Reimbursement-System.git


> Make AWS account 
> Download MariaDB
> Connect MariaDB to AWS Database
> Set up tables in MariaDB
> Run Javalin
> Copy/Paste Login.Html in Browser

`DROP TABLE IF EXISTS employee;
DROP TABLE IF EXISTS reinbursement;
DROP TABLE IF EXISTS reinbursement_employee;

CREATE TABLE employee
(
	crew_number INT NOT NULL,
	crew_email VARCHAR(200),
	password VARCHAR (200),
	isManager ENUM ('Captain', 'Crew Memeber'),
	
	CONSTRAINT employee_pk PRIMARY KEY(crew_number)
	);

CREATE TABLE reinbursement
(
	case_number INT AUTO_INCREMENT,
	description VARCHAR(200),
	balance DECIMAL (10,2),
	status ENUM ('Approved','Denied','Standby'),
	CONSTRAINT reinbursement_pk PRIMARY KEY(case_number)
	
);
`
## Usage

- Enter employee credentials when logging in to submit reimbursements.
- Enter in Amount and description.
- Click submit
- Logout

- Enter Manager credentials to Approve/Decline reimbursements.
- Enter case number and Approve/Decline.
- Click Submit.




