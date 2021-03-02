---
layout: page
title: HW03 Defensive Programming
permalink: /assignments/hw3
parent: Assignments
---

# Homework 2
In this homework, you will practice writing a Python application, dealing with uncleaned data, handling potential errors, and using assert statements.  Please read the entire assignment in full before you begin. You might find some helpful information in the Resources section. 

## Learning goals
- Identify problems in data programmatically
- Write code to handle errors
- Write asserts to catch future errors
- applying previous skills, git/github and reading files

## Tasks

You will be asked to perform the following series of tasks:
- Pull Changes from your repository
- Confirm that you can run the starter code
- Find issues in the uncleaned csv file
- mitigate issues computationally

#### Pull Changes from your repository
We have pushed the starter code and input data to each for your repositories, specifically to a folder titled HW3 in your homework-username directory.

#### Confirm that you can run the starter code
You should start by confirming that you can run the starte code we provided for you in your repositories. It is called 'cleanCSV.py'. When you run it, it should read the input csv file ('input.csv') and write an output csv file ('output.csv').  The starter code should perform all the file reading and writing. When you first run it the output file will be the same as the input file. 

#### Identify problems in the uncleaned csv file
You should identify the problem we have injected into the uncleaned csv file. We have added two examples of nine types of problems to the file (a total of 18 problems). You should identify them all.  Since the file is large you will be most effective in finding the problems if you search for them programmatically. You might also want to write asserts to help identify problems. 
To assist you, we have provided a file, `problems.md`, which gives a short description of each type of problem. Once you find the problems, you should write their line numbers under the appropriate category in problems.md.


#### mitigate issues computationally
Modify starter code file so it outputs a cleaned csv. You should not repair the mangled .csv by hand.  Your program should output as much of the original data as possible, but repair the problems you identified in one of the ways we discussed in class: 1) replace garbled data with default values 2) use an average of other values in the column 3) remove extraneous content 4) adds missing content 5) perform a bespoke/one-off correction. *If the input data is irredeemable it is also okay to remove the line.* 

For each of the problems you identified above, write a very short (e.g. one sentence) justification of the fix to your program. These justifications should explain why the fix you wrote was appropriate for the problem. Write these justifications immediately after each problem in problems.md. 

## Resources
https://www.w3schools.com/python/ref_keyword_assert.asp#:~:text=The%20assert%20keyword%20is%20used,False%2C%20check%20the%20example%20below.
https://www.w3schools.com/python/ref_func_isinstance.asp
https://www.askpython.com/python/examples/add-a-newline-character-in-python
https://docs.python.org/3/library/datetime.html
https://www.w3schools.com/python/python_casting.asp

## Tips and Suggestions
You might want to combine automated analysis with manual inspection of the input file
Add assert statements to check for correct types (ie what type should state be?)
Use print statements
The 'len()' function can check the length of a string (e.g. 'len(“cat”) == 3')
The isinstance() function can check the type of an input (e.g. 'assert isinstance(5, int)')
You can change the type of variables (e.g. int(“4”) become 4)
As much as possible, try to avoid hard-code to catch errors.  Your code should be able to catch the errors on other sets of data.  For example, do not just say: if row # = 42, don’t include in new csv.  We want you to use logic, so your code can be applied to any different csv files and catch the incorrect data.

## Deadlines and Deliverables
All deliverables should be committed and pushed to the main branch of your repository on GitHub.  Both are due Thursday, Feb 25th. The files that should be included in your repository (in the subdirectory hw3) should be: 1) problems.md 2) cleanCSV.py 3) input.csv 4) output.csv. Additional files are okay, but these are required.
