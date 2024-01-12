---
layout: page
title: HW03 Defensive Programming
permalink: /assignments/hw3
parent: Assignments
---

# Homework 3 

**Part (a) Due Thursday Feb 10th at 3:05pm EST**{: .label .label-red } 
**Part (b) Due Thursday Feb 17th at 3:05pm EST**{: .label .label-red }

In this homework, you will practice writing a Python application, dealing with uncleaned data, handling potential errors, and using `assert` statements. Please read the entire assignment in full before you begin. You might find some helpful information in the [Resources section](#resources). 

__NOTE: this homework contains two parts (a and b) with separate due dates.__ The main purpose is to let instructors give you feedback to help you successfully complete the homework.

## Learning goals

- Identify problems in data programmatically
- Write code to handle errors
- Write `assert`s to catch future errors
- Applying previous skills: `git`/GitHub and reading files

## Tasks

You will be asked to perform the following series of tasks for part (a):

- Create a `hw3` folder in your homework monorepo
- Download the input CSV file
- Create a script with some starter code for reading and writing files
- Find one issue in the uncleaned `.csv` file

Here are the tasks for part (b):

- Find the rest of the issues in the uncleaned `.csv` file
- mitigate issues computationally

### Create a `hw3` folder in your homework monorepo 

In your `crafting-software-hw-<username>` directory (the same repo you used for the last homework), create an empty directory called `hw3`. Please also include a `README.md` file in `hw3` with the following information:

* The title of the homework (`# Homework 3`)
* Your name and Andrew ID

A `.md` file is written in the Markdown syntax. Refer to this [quick reference](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) to learn more about how to format your `README` file and any conversations on GitHub.

### Download the input CSV file

We provided a CSV file with some errors. 

__Download the file (`input.csv`) here__: 
<https://gist.githubusercontent.com/wodeni/c3460ead276a2ea87ad7f7fcc0dda246/raw/a790d28f66971ed1c70f43eb475907018705a7d1/input.csv>

Please put the file in `hw3`. Throughout this homework, you will identify the problems in this file and fix them computationally in a Python program.

### Write some starter code for reading and writing files

Create a Python file called `cleanCSV.py` in the `hw3` directory. For this step, you only need to implement the following funcionalities:

* Read the input csv file (`input.csv`) 
* Write an output csv file (`output.csv`)
* When you run `cleanCSV.py`, the output file should be exactly the same as the input file. 

### Identify problems in the uncleaned CSV file

You should identify the problem we have injected into the uncleaned CSV file. We have added two examples of nine types of problems to the file (a total of 18 problems). You should identify them all.  Since the file is large, you will be most effective in finding the problems if you search for them programmatically. You might also want to write `assert`s to help identify problems. 

To assist you, here is a full list of problems in `input.csv`, with a short description of each type of problem. There are 2 instances of each of the problems below:

* Full state name
* Invalid state code 
* Extra comma
* Date out of range
* Decimal instead of an Integer
* Add letter added to an Integer
* NumString in the place of an Integer
* CharString in an Integer
* Missing newline

You should paste this list into your `README.md` and add your findings as you work through this homework. Once you find an instance of a problem type, you should write the line numbers where the instance occured under the appropriate category in `README.md`.

__For part (a), find one of those problems. For part (b), you will find all problems in `input.csv` and fix them computationally.__
### Mitigate issues computationally

Modify `cleanCSV.py` so it outputs a cleaned csv. You should not repair the mangled `.csv` by hand. Your program should output as much of the original data as possible, but repair the problems you identified in one of the ways we discussed in class: 

1. Replace garbled data with default values 
2. Use an average of other values in the column 
3. Remove extraneous content 
4. Add missing content 
5. Perform a bespoke/one-off correction. *If the input data is irredeemable it is also okay to remove the line.* 

For each of the problems you identified above, write a very short (e.g. one sentence) justification of the fix to your program. These justifications should explain why the fix you wrote was appropriate for the problem. Write these justifications immediately after each problem in `README.md`. 
## Resources
* <https://www.w3schools.com/python/ref_keyword_assert.asp>
* <https://www.w3schools.com/python/ref_func_isinstance.asp>
* <https://www.askpython.com/python/examples/add-a-newline-character-in-python>
* <https://docs.python.org/3/library/datetime.html>
* <https://www.w3schools.com/python/python_casting.asp>

## Tips and Suggestions
* You might want to combine automated analysis with manual inspection of the input file.
* Add `assert` statements to check for correct types (ie what type should state be?)
* Use `print` statements
* The `len()` function can check the length of a string (e.g. `len(“cat”) == 3`)
* The `isinstance()` function can check the type of an input (e.g. `assert isinstance(5, int)`)
* You can change the type of variables (e.g. `int(“4”)` become `4`)
* As much as possible, try to avoid hard-code to catch errors. Your code should be able to catch the errors on other sets of data. For example, do not just say: `if row # = 42`, don’t include in new CSV. We want you to use logic, so your code can be applied to any different CSV files and catch the incorrect data.

## Deadlines and Deliverables

__Due Dates__: 

* Part (a): Thursday Feb 10th at 3:05pm.  
* Part (b): Thursday Feb 17th at 3:05pm.  

You may use up to two (2) late days for each part. To use a late day, simply message us on Slack to let us know that you will be using a late day.

__Deliverable__: For this assignment, the files that should be included in your repository (in the subdirectory `hw3`) should be: 

1. `README.md`
2. `cleanCSV.py`
3. `input.csv`
4. `output.csv`

When you are ready to submit part (a), you should create a new tag, your tag should be `3.0-alpha` (for HW3 [alpha release](https://en.wikipedia.org/wiki/Software_release_life_cycle#Alpha)). 

When you are ready to submit part (b), create a new tag called `3.0` (for HW3 final version). 

Here's a quick guide to `git tag`: <https://git-scm.com/book/en/v2/Git-Basics-Tagging>.

All deliverables should be committed and pushed to the `main` branch of your repository on GitHub.
