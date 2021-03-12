---
layout: page
title: HW05 Advanced Data Management System
permalink: /assignments/hw5
parent: Assignments
---

# Homework 5
In this homework, you will continue working with your python application that interacts with an RDBMS (Relational Database Management System). 
This work will build on your HW4 solution.
Please read the entire assignment in full before you begin. You might find some helpful information in the Resources section.

## Learning goals
- Demonstrate ability to use database features like views, transactions, and indexes
- Generate random data for testing database performance
- Applying previous skills, git/github and reading files

## Tasks

You will be asked to perform the following series of tasks:
- Create a view in your table
- Create a transaction to make at least two changes do the DB in a single transaction
- Create random data to test our database
- Join existing data with random data
- Add an index to your table and measure a change in performance

#### Create a view in your table
You should create a view of a query. Your view should show the population for each state for all ages, and all ages only. 
You should name your view something that makes it clear that it is all ages population.  
You should perform these commands via a python script.  
You can start with your answer to hw4, and add the creation of a view.  
HINT: the “ OR REPLACE” keyword might come in handy to be able to re-run your script multiple times.
 
#### Create a transaction to make at least two changes do the DB in a single transaction
You should create a transaction in your database.  Your transaction should alter at least two rows in the transaction. 
You may choose which two rows to alter.  You should print out the values of the rows first, 
then perform the transaction, then print the new values. This should also be done in your python script.

#### Create random data to test our database
In order to be able to test an index, we will need more data. 
To do this, you should create a new table, and fill it with random data. This can be done with the following SQL commands.

CREATE TABLE rand_state_data(
	rand_id SERIAL PRIMARY KEY,
	rand_state_code numeric NOT NULL,
	rand_value NUMERIC NOT NULL
);

INSERT INTO rand_state_data (rand_state_code,rand_value)
SELECT  ((random() * 49)+1)::integer,
       ((random() * 99) + 1)::integer
FROM generate_series(1, 10000000);

NOTE: this only needs to be done one time, and it might take a while to run on your computer. 
You can do this directly from SQL, you do not need to do this from python.

#### Join existing data with random data
You should count the number of random values that are greater than 80 for each state in your census data table.  
Your number will be slightly different than other students in the class.  
This should be done via a single SQL statement.  
You should join both tables, and count the number with a rand_value greater than 80. 
This query might take a while to run.  You should run this query via your python script.

#### Add an index to your table and measure a change in performance
We will speed up this query using at least one index.  
You should first run the query you created in the step above without the index created. 
You should observe and record the exact timing of the run with the “EXPLAIN ANALYZE” feature.  
Then, you should create at least one index that you think will speed it up.  
Then you should re-run the query with EXPLAIN ANALYZE with the index, and record what the speed up was.  
You should try adding a second index, and observe if there is a performance gain.   
You should copy the output of your script, including the recorded exectution times before and after the index, 
and commit them to your repo in a text file called SQLResults.txt. HINT: You might need to delete the index if you want to try doing this several times.


## Resources
https://www.postgresql.org/docs/current/sql-createview.html
https://www.postgresql.org/docs/current/transaction-iso.html
https://www.postgresql.org/docs/13/sql-createindex.html


## Deadlines and Deliverables
The deliverable should be committed and pushed to the main branch of your repository on GitHub. 
It is due Thursday, March 18th. The files that should be included in your repository (in a subdirectory hw5) should be: 1) hw5.py  2) SQLResults.txt. Additional files are okay, but these are required.



