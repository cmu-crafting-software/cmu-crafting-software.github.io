---
layout: page
title: HW02  Reading Data
permalink: /assignments/hw2
parent: Assignments
---

# Homework 2 **Due Tuesday Feb 16th at 4pm EST**{: .label .label-red }
In this homework you will practice writing a python application, as well as reading data from various sources. Please read the entire assignment in full before you begin. You might find some helpful information in the Resources section. 

## Learning goals
- Write a simple “hello world” python program
- Run python application
- Read in data from a CSV file
- Store data in the application 
- Calculate some basic statistics from data collected


## Tasks
You will be asked to perform the following series of tasks:
- Clone Homework Repo via GitHub Classroom.
- Create and run a  “Hello World” program
- Read csv file of COVID data
- Print COVID Data
- Calculate the sum and average of any two columns in the data set
- Read data directly from the covid data tracking project using their API
- Show correctness by calculating a value available on the website, to confirm correctness

#### Clone Homework Repo via GitHub Classroom.
Your first step for this project is to configure your repository that you will be working in for this assignment. You should create a repository via Github classroom at this link: https://classroom.github.com/a/yFf56mVO
You will be committing your solutions to this repo for all this homework.

#### Create and run a  “Hello World” program
In recitation you will be performing this task.  You may simply copy your recitation solution for this.  You should commit your solution as a single commit to your Homework Repository. 

#### Read csv file of COVID data
You should write a small program in python that will read data from a .csv file.  In this class, we will be using the .csv file of data from the COVID tracking project (https://covidtracking.com/). You can find the CSV file here: https://covidtracking.com/data/download
We suggest you work with the national summary data.
You should download the csv file and commit it to your homework repository.  Then, you should write a small program to read each line of the CSV file into your program.
You should push a commit to your repository with a clear name once you have reached this point.

#### Print COVID Data
The next step is to simply print out the data using the “print” function in your application.  Once you have achieved this, you should commit this change to your repository, and push it to your repo.

#### Calculate the sum and average of any two columns in the data set
The data in the .csv is documented by the first row in the dataset. You should choose one of the columns with numerical values, and calculate the sum of all the numbers.  Then, you should calculate the average of another numerical column.  
To confirm these are the correct values, you should import the csv into a spreadsheet (excel, google sheets, etc), and calculate the same values, and compare them.  You should then commit this code. In the commit message, you should specify which columns you used, and what the values were.

#### Read data directly from the covid data tracking project using their API, using requests API
Another way to get the data from the covid tracking project is to use their API (Application Programming Interface).  You can find the API documented here: https://covidtracking.com/data/api
To get the data from the API, you will need to make a request.  To make the API call, you should use the requests API: https://requests.readthedocs.io/en/master/
NOTE: installing requests might go smoothly, or it might be difficult. Please don’t hesitate to reach out, as there are lots of small things that could make this step go wrong.
To confirm that you have retrieved the data, you should print it out.  Then, you should commit and push this to your homework repository

#### Show correctness by calculating a value available on the website, to confirm correctness
To verify that you are using the data correctly, you should find a value on the website that you can calculate from the API data.  You should then calculate the value, and compare it against the value on the site.  Your commit message should show what the value is, and what confirm what your calculated value is.

## Resources

Some Resources that might be helpful: 
Running python code in virtual env
Reading a csv in python: https://realpython.com/python-csv/, https://stackoverflow.com/questions/11310248/find-number-of-columns-in-csv-file, https://docs.python-guide.org/starting/install3/osx/

Pip installing requests: https://requests.readthedocs.io/en/master/user/install/, https://stackoverflow.com/questions/18363022/importerror-no-module-named-pip

Using requests: https://realpython.com/python-requests/, https://stackoverflow.com/questions/31126596/saving-response-from-requests-to-file, https://learning.postman.com/docs/sending-requests/requests/#creating-requests


## Tips and Suggestions
To help make sure you are getting the API data correctly, you might want to use the Postman tool.
If you copy code from the internet, add a comment to attribute it.

## Deadlines and Deliverables
Due Date: Tuesday Feb 16th at 4pm.  
You may use up to two (2) late days, out of six total.  To use a late day, simply message us on slack to let us know that you will be using a late day.
Deliverable: For this assignment, you have one deliverable.
You should commit the code you have written to your repository as you go along. When you are ready to submit, you should create a new tag, your tag should be 2.0 (for HW2). (https://git-scm.com/book/en/v2/Git-Basics-Tagging)



## Assignment Review
Because this is a new class, we are asking you to fill out a short survey to help us calibrate the homeworks.  This survey is ungraded, but your input will be very valuable for us in improving the course both for this semester, and for future years. 
https://docs.google.com/forms/d/e/1FAIpQLSe1v3TKk8_g4IB6P2DhQ3MUgPZJC9GCzqBoLZuzEVaM9aKguA/viewform


## Grading

The total assignment is worth 100 points.

| Item        | Points      |
| ----------- | ----------- |
| Program compiles and runs |  30    |
| Reads CSV data correctly |   30   |
| Reads API data correctly |   30   |
| Correct git/GitHub usage |  10    |
| ----------- | ----------- |
| Total       | 100         |





