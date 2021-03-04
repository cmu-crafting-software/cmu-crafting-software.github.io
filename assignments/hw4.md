---
layout: page
title: HW04 Using a Relational Database Management System
permalink: /assignments/hw4
parent: Assignments
---

# Homework 4
In this homework, you will build a Python application that interacts with the PostgreSQL relational database managements system. You will create a database, read data from two APIs, insert the data into the database, and queries from the database. Please read the entire assignment in full before you begin. You might find some helpful information in the Resources section. 

## Skills demonstrated
- Design tables and their relationships that are appropriate for a data set.
- Write code to define a database.
- Insert data into a database.
- Query data from a database.

## Tasks

### 1. Retrieve COVID vaccination and state population data
- Use Python to retrieve the 2019 Census estimated population of each state for each of the following age groups: Age 85 years and older, Age 80 to 84 years, Age 75 to 79 years, Age 70 to 74 years, Age 65 to 69 years, Age 60 to 64 years, Age 55 to 59 years, Age 50 to 54 years, Age 45 to 49 years, Age 40 to 44 years, Age 35 to 39 years, Age 30 to 34 years, Age 25 to 29 years, Age 20 to 24 years, Age 15 to 19 years, Age 10 to 14 years, Age 5 to 9 years, Age 0 to 4 years. Use the Census "charagegroups" API. Refer back to the in-class from February 12 for examples of use.
- Use Python to retrieve the COVID testing data for every state from each day using [The Covid Tracking Project](https://covidtracking.com/). It's probably easiest to load the data from [a file](https://covidtracking.com/data/download/all-states-history.csv), but you can also use the API if you prefer. You will ultimately store this data in the database. For now, read from the APIs and files and assign the result to Python variables. 

### 2. Create database tables
- Design a reasonable table layout for the data retrieved in the previous step. Use at least two tables and choose reasonable relationships between tables. Every table should have a primary key. Use foreign key(s) to preserve referential integrity. 
- Write SQL data definition language (DDL) code to create the tables you designed. Be sure to choose reasonable datatypes for each column and use primary and foreign keys where appropriate.
- At the minimum your tables should include the following columns across all the tables. You can discard other data from step 1 or add additional columns: state_code, state_name, age_group_id, age_group_description, population, test_date, negative_increase, positive_increase, total_test_results_increase.
- Save your SQL DDL code in a file called `createTables.sql`.
- Create the tables in your database using the SQL DDL code you wrote.

### 3. Insert the retrieved data into tables
- Use Python to insert all of the data retrieved in step 1 above into the database defined in Step 2.

### 4. Query the database
Use Python to query the database and print out answers to the following below. Feel free to use any combination of SQL queries and Python code to answer the question. 
- Which state has the lowest percentage of people aged 85 years and older? Print the name of the state, the percentage, to 85+ population, and the total population. 
- Which state had the most positive tests per capita in a single day? Print the name of state, the day, the number of positive tests per capita, the population of the state, and the number of positive tests.
- The Python code you wrote in this step, step 1, and step 3 should be save in a file called `readAndInsert.py`.

## Resources
- https://github.com/cmu-crafting-software/in-class/tree/main/feb-12-apis
- https://api.census.gov/data/2019/pep/charagegroups/variables.html
- https://api.census.gov/data/2019/pep/charagegroups/variables/AGEGROUP.json

## Deadline and deliverables
The Homework is due at 4pm EST on Tuesday, March 9. Please hand in the following files by pushing them to your homework repository in a directory called HW4:
- `creatTables.sql`
- `readAndInsert.py`


