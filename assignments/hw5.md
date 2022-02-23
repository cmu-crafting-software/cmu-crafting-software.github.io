---
layout: page
title: HW05 Pandas
permalink: /assignments/hw5
parent: Assignments
---

# Homework 5

**Due Thursday Mar 3rd at 3:05pm EST**{: .label .label-red } 

In this homework, you will be working with Pandas in a Juypter notebook. 

Please read the entire assignment in full before you begin. You might find some helpful information in the [Resources](#resources) section.

## Learning goals

- Import data into a notebook
- Answer questions by analyzing the data frame
- Join two data frames
- Follow best practices for notebook use

## Tasks

For this assignment, you will be doing pandas tasks, and you will share your solution in a Jupyter notebook.

You will be asked to perform the following series of tasks, all in Jupyter notebook:
- Import data into a dataframe from your SQL Database
- Add a column to the covid data that indicates what day of the week each day represents
- Find the average number of increase in test results by day of the week (i.e., the avg number of test results increase on mondays, tuesdays, etc)
- Join data frames
- Add a new column to the data frame that is the per capita hospitalized number (hospitalizedCurrently/ total number of residents).
- Avoid hidden state errors

### Import data into a dataframe from your SQL Database

You should import the COVID data and the Census data from your database.  You may reuse code from the previous homework, if you find that helpful.  You should import each dataset into a dataframe each, and you will use these dataframes for the rest of the homework.

### Add a column to the covid data that indicates what day of the week each day represents

You should add a new column to the covid dataframe that represents the day of the week.  You can use strings or numbers to represent the day of the week.  (its ok if you want to do both a number and a string). 

### Find the average number of increase in test results by day of the week (i.e., the avg number of test results increase on mondays, tuesdays, etc).   

Using pandas, you should calculate (and print) the average number of increased tests result by day of the week.  NOTE: you might want to plot this data. We will talk about visualizations in depth later on, but for now, you may plot the data if you want, but you are not required to.

### Join data frames

Join both dataframes, the covid and the census data.  You should join them on states, as we have done previously. You should also create new dataframe that you can use for the following question.

### Add a new column to the data frame that is the per capita hospitalized number (hospitalizedCurrently/ total number of residents).

Add a new column to the combined dataframe that is per capita hospitalizations.  

### Avoid hidden state errors

Throughout this homework, you should follow best practices as we described in lecture. Specifically, you should avoid relying on hidden state.   This means that you should be able to run your cells in any order, and get the same results. 

You should not have any 2 cells that write to the same object in shared state, but you may read the same object several times.

## Bonus Challenge: 

Calculate a statistical test to see if there is a statistical difference between weekend deaths vs weekday deaths.

## Resources

* <https://pandas.pydata.org/docs/user_guide/merging.html>
* <https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.sort_index.html>
* <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html>
* <https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.groupby.html>

## Tips and Suggestions
To calculate the day of the week, consider reading the datetime documentation: https://docs.python.org/3/library/datetime.html
To calculate information by day of the week, considering which information to make the index of the DataFrame and the various index operations available


## Deadlines and Deliverables

__Due Date__: Thursday Mar 3rd at 3:05pm EST

The deliverable should be committed and pushed to the main branch of your repository on GitHub. Your notebook file (i.e. .ipynb) file should be committed and pushed to your homework repository in a `hw5` subdirectory.
