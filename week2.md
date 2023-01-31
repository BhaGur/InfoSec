# Week 2 Assignments
This file tasks for the assignments for Information security course. It conatins the step I did while performing the tasks for the assignment.

## Summary of the OWASP top-10 list
### Security misconfiguration
*	A lapse in the security architecture causes vulnerability of applications
*	Main causes for security main configuration are missing of appropriate security in application
*	It may happen also if unnecessary features are enabled or installed or the software used are out of date
*	If the default accounts and passwords are unchanged
*	These shortcomings may be used by attackers to access the server thorough default logins and take control of the server
*	Out of date software are easy targets for attackers through which they can find, download, and reverse the code.
*	Attacker can gain access of the sensitive data about other users in the server or the cloud
*	The best way to avoid these shortcomings is proper installation of secure and updated patch management process
*	Hardening of security and segmentation of the application architecture
*	Removal of unwanted or unused features

### Vulnerable and Outdated components
*	This vulnerability concerns with the versions of the components on both client and server side.
*	This usually is because of the unsecure, out of date software in the server including the OS, application server, DATABASE, an all components
*	Not testing the compatibility of updated, upgraded or patched library leaving organization exposed to vulnerabilities
*	Components run with same privileges as the application, which leads to a serious consequences.
*	It helps attackers to find unpatched or misconfigured systems, through which they exploit the application
*	Removal of unused software or programs and files can patch the application
*	Components should be obtained through secure links and continuously monitor the components on both server and client side.

### Injection
*	The vulnerability occurs as a result of unvalidated, unfiltered user-supplied data
*	Use of hostile data in object-relational mapping search parameters
*	SQL or commands containing malicious data
*	Attackers inputs vulnerable SQL calls which returns all the records from database.
*	They can modify, delete or store data in the database
*	To prevent injection, application should use safe API
*	Remove any unwanted injection by limiting control in SQL queries

## Episode - 124 Synthetic Remittance
* This episode told a real story about get-rich-quick scheme
* A Lithuanian man named Evaldas Rimasaukas conducted a Business E-mail Compromise (BEC) scam that made big companies like Facebook and Google to make fake payments to him rather than another business that worked with those companies
* He and his team bought a fake domain of a company and made fake invoices which were sent to facebook and google
* The team researched about the payment mechanism of those companies and also copied the real invoice that the partner business used
* The bank account was also changed so the money will go to his bank account
* The money once recieved would be transfered to other bank all over the world to make it hard to trail the money
* The security system was not breached or compromised in this instance but the method was spear phising or spoofed emails.
* The business needs to be aware of such scams
* If a big corporations can be a victim of such scams, it is likely that small business would also be a target
* Security is not just about building a secure architecture but also being cautiuos about other forms of scams

## CVE-2022-46689
*	A vulnerability seen in Apple macOS which abled an app to execute arbitrary code with kernel privileges.
*	The severity of the CVE was 7.0 high according to CVSS version 3.x. The impact score was 5.9.
*	Attack vector was Local and Attack complexity was high.
*	It required user interaction.
*	It affected software configurations in safari, ipados, iphone_os, macos.

## SQLZOO
### 0 SELECT basics
*	The chapter dealt with introducing some simple queries
*	The chapter was easy as the instructions were given and we just needed to make some changes in the queries to get the required answer
*	After the chapter was completed, I did the quiz where I was to select correct queries
<img src="https://github.com/BhaGur/InfoSec/blob/main/sqlzoo1.png" width="400" height="150"> 

### 1 SELECT name (voluntary)
*	The chapter deals with use of ‘LIKE’ in queries
*	I had to modify the given query to find the answer
<img src="https://github.com/BhaGur/InfoSec/blob/main/sqlzoo2.png" width="400" height="150"> 

*	The first 10 queries were easier ones but the last few were a bit harder.

### 2 SELECT world
*	The chapter deals with the use of SELECT in queries
*	I had to write queries to find correct answers from the WORLD table
*	I was required to do till sub task 5 but I did till subtask 10.
<img src="https://github.com/BhaGur/InfoSec/blob/main/sqlzoo3.png" width="400" height="150"> 
<img src="https://github.com/BhaGur/InfoSec/blob/main/sqlzoo4.png" width="400" height="150"> 


## WEBGOAT Injection (Intro)
*	Using SQL queries for managing relational databases and perform operations on the data in the database
*	Data Manipulation Language (DML) is the manipulation of the SQL statement used by attacker to manipulate the database
*	After each sub chapter, I had to do an assignment. I had to update a SQL query as below.
<img src="https://github.com/BhaGur/InfoSec/blob/main/webgoat1.png" width="400" height="150"> 

*	Another task required us to add a column to the employees table. I completed the task as given in the image below
<img src="https://github.com/BhaGur/InfoSec/blob/main/webgoat2.png" width="400" height="150"> 

*	Another task was to grant permission to a user group which I completed as below
<img src="https://github.com/BhaGur/InfoSec/blob/main/webgoat3.png" width="400" height="150"> 

*	SQL injection exploits by modifying the input and inputting malicious code and allows attackers to temper with existing data
*	Another task was to retrieve data by selecting an sql injection which I did as below
<img src="https://github.com/BhaGur/InfoSec/blob/main/webgoat4.png" width="400" height="150"> 

*	The injection task was completed as below. First I tried to input the code in Login_Count. The solution was not correct. Then I input the code in the User_id, then the injection worked and I was able to get the data of the user from the database
<img src="https://github.com/BhaGur/InfoSec/blob/main/webgoat5.png" width="400" height="150"> 
<img src="https://github.com/BhaGur/InfoSec/blob/main/webgoat6.png" width="400" height="150"> 

*	In the next task, I had to retrieve data of users. I used the following query in the input
<img src="https://github.com/BhaGur/InfoSec/blob/main/webgoat8.png" width="400" height="150"> 
<img src="https://github.com/BhaGur/InfoSec/blob/main/webgoat7.png" width="400" height="150"> 

* After that I was able to compromise the confidentiality of data and see the salary of other employees
* In this task I had to set the salary of Smith to what is in the database. I used the following code and I was able to increase the salary of Smith with userid number = 37648.
<img src="https://github.com/BhaGur/InfoSec/blob/main/webgoat10.png" width="400" height="150"> 

*	I was able to drop table with the following code and was successful.
<img src="https://github.com/BhaGur/InfoSec/blob/main/webgoat11.png" width="400" height="150"> 
