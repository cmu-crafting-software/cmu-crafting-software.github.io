---
layout: page
title: HW04 Pandas
permalink: assignments/hw4
parent: Assignments
---

# Homework 4 **Due Friday Feb 28th at 2pm EST**{: .label .label-red }

In this homework, you will be working with Pandas in a Juypter notebook.

Please read the entire assignment in full before you begin. You might find some helpful information in the [Resources](#resources) section.

## Learning goals

- Import data into a notebook
- Answer questions by analyzing the dataframe
- Join two dataframes
- Follow best practices for notebook use

## Tasks

For this assignment, you will be doing Pandas tasks, and you will share your solution in a Jupyter notebook.

You will be asked to perform the following series of tasks, all in Jupyter notebook:

- Import data into dataframes from a CSV file (COVID vaccine and case data) and via a REST API (census data).
- Add a column to the vaccination data that indicates what day of the week each day represents
- Find the average number of increase in cases by day of the week (i.e., the avg number of cases increase on mondays, tuesdays, etc)
- Join dataframes
- Add a new column to the dataframe that is the per capita hospitalized number (hospitalizedCurrently/ total number of residents).
- Avoid hidden state errors

### Create homework repo via GitHub Classroom

Your first step for this project is to create your repository that you will be working in for this assignment. You should create a repository via GitHub Classroom using this link: <https://classroom.github.com/a/ODOEMS2s> After accepting the homework, GitHub Classroom will create a repo named `cmu-crafting-software/2025-homework04-$YOUR_GITHUB_ID`.

You'll need to install a couple packages. To do so, use [uv](https://docs.astral.sh/uv/):

```sh
uv init
uv add ipykernel pandas requests
```

When you run these commands, VS Code should ask if you want to activate the virtual environment in the `.venv` folder that uv just created; click **Yes**. If you discover that you need more packages as you're working on the rest of this assignment, you can just use [`uv add`](https://docs.astral.sh/uv/concepts/projects/dependencies/#adding-dependencies) in your terminal again.

(If any of the above terminal commands don't work, run the VS Code **Codespaces: Rebuild Container** command and then try again.)

Please also create a `README.md` file with the following information:

- The title of the homework (`# Homework 4`)
- Your name and Andrew ID

### Import data into dataframes

For the rest of this assignment, you will work inside of a Jupyter notebook. Create a Jupyter notebook file and open it in VS Code.

You should import the COVID data from this CSV file:

<https://gist.githubusercontent.com/wodeni/2d838d8241b229b63aa2a4f1a044e994/raw/12b1bcf27d06ed9c864f03933333f76918781c3f/state.timeseries.csv>

Use the query from [Recitation 2](https://github.com/cmu-crafting-software/recitations-25/tree/5fe184e451ef1ef4457637d3ad8eb1b457aaab2d/recitation-2) and the [`requests` library](https://docs.python-requests.org/en/latest/) to request the census data and load it into a dataframe:

```
https://api.census.gov/data/2019/pep/charagegroups?get=NAME,POP&for=state:*
```

You should import each dataset into a dataframe each, and you will use these dataframes for the rest of the homework.

### Add a column to the vaccine data that indicates what day of the week each day represents

You should add a new column to the vaccine dataframe that represents the day of the week. You can use strings or numbers to represent the day of the week. (It's okay if you want to do both a number and a string).

### Find the average number of case increase by day of the week

Using pandas, you should calculate (and print) the average number of increased cases by day of the week. NOTE: you might want to plot this data. We will talk about visualizations in depth later on, but for now, you may plot the data if you want, but you are not required to.

### Join dataframes

Join both dataframes, the vaccine and the census data. You should join them on states, as we have done previously. You should also create new dataframe that you can use for the following question.

### Add a new column to the dataframe that is the per capita vaccination number

Add a new column to the combined dataframe that is per capita vaccination (`vaccination / total number of residents`) for each state.

### Avoid hidden state errors

Throughout this homework, you should follow best practices as we described in lecture. Specifically, you should avoid relying on hidden state. This means that you should be able to run your cells in any order, and get the same results.

You should not have any 2 cells that write to the same object in shared state, but you may read the same object several times.

## Bonus Challenge:

Calculate a statistical test to see if there is a statistical difference between weekend vs weekday cases.

## Resources

- <https://pandas.pydata.org/docs/user_guide/merging.html>
- <https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.sort_index.html>
- <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html>
- <https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.groupby.html>

## Tips and Suggestions

To calculate the day of the week, consider reading the `datetime` documentation: <https://docs.python.org/3/library/datetime.html>
To calculate information by day of the week, considering which information to make the index of the DataFrame and the various index operations available

## Deadlines and Deliverables

**Due Date**: Friday Feb 28th at 2pm EST

The deliverable should be committed and pushed to the main branch of your repository on GitHub. Your notebook file (i.e. `.ipynb`) file should be committed and pushed to your homework repository.
