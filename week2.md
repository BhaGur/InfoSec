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

### 1 SELECT name (voluntary)
*	The chapter deals with use of ‘LIKE’ in queries
*	I had to modify the given query to find the answer
*	The first 10 queries were easier ones but the last few were a bit harder.

### 2 SELECT world
*	The chapter deals with the use of SELECT in queries
*	I had to write queries to find correct answers from the WORLD table
*	I was required to do till sub task 5 but I did till subtask 10.

## WEBGOAT Injection (Intro)
*	Using SQL queries for managing relational databases and perform operations on the data in the database
*	Data Manipulation Language (DML) is the manipulation of the SQL statement used by attacker to manipulate the database
*	After each sub chapter, I had to do an assignment. I had to update a SQL query as below.
*	Another task required us to add a column to the employees table. I completed the task as given in the image below
*	Another task was to grant permission to a user group which I completed as below
*	SQL injection exploits by modifying the input and inputting malicious code and allows attackers to temper with existing data
*	Another task was to retrieve data by selecting an sql injection which I did as below
*	The injection task was completed as below. First I tried to input the code in Login_Count. The solution was not correct. Then I input the code in the User_id, then the injection worked and I was able to get the data of the user from the database
*	In the next task, I had to retrieve data of users. I used the following query in the input
* After that I was able to compromise the confidentiality of data and see the salary of other employees
* In this task I had to set the salary of Smith to what is in the database. I used the following code and I was able to increase the salary of Smith with userid number = 37648.
*	I was able to drop table with the following code and was successful.
