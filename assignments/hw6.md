---
layout: page
title: HW06 Visualization
permalink: assignments/hw6
parent: Assignments
---

# Homework 6 **Due Monday Mar 31st at 2pm EDT**{: .label .label-red }

In this homework, you will be working with Altair in a Juypter notebook.
Please read the entire assignment in full before you begin. You might find some helpful information in the Resources section.

## Learning goals

- Understand Altair, Data Types, Graphical Marks, and Visual Encoding Channels
- Make informative graphs using data visualizations we discussed
- Interact and transform the data
- Iterate over graphs and select features that best show the data

## Create homework repo via GitHub Classroom

Your first step for this project is to create your repository that you will be working in for this assignment. You should create a repository via GitHub Classroom using this link: <https://classroom.github.com/a/KoSh4BnE> After accepting the homework, GitHub Classroom will create a repo named `cmu-crafting-software/2025-homework06-$YOUR_GITHUB_ID`.

You'll need to install a couple packages. To do so, use [uv](https://docs.astral.sh/uv/):

```sh
uv init
uv add ipykernel
```

When you run these commands, VS Code should ask if you want to activate the virtual environment in the `.venv` folder that uv just created; click **Yes**. If you discover that you need more packages as you're working on the rest of this assignment, you can just use [`uv add`](https://docs.astral.sh/uv/concepts/projects/dependencies/#adding-dependencies) in your terminal again.

(If any of the above terminal commands don't work, run the VS Code **Codespaces: Rebuild Container** command and then try again.)

Please also create a `README.md` file with the following information:

- The title of the homework (`# Homework 6`)
- Your name and Andrew ID

## Tasks

For this assignment, you will be doing Altair tasks, and you will share your solution in a Jupyter notebook.

You will be asked to perform the following series of tasks, all in jupyter notebook:

- Import the same data you used for HW4 (COVID and census. You may copy and paste that code).
- In a cell, write a comment that gives an example of Nominal, Ordinal, Quantitative, and Temporal data using the columns in the COVID dataset.
- Start by creating a default graph where you visualize the relationships between two columns in the data using a default graph (using `mark_point`).
- Modify the previous mark_point graph and use visualization elements and arguments to make the graphs easier for users to read and understand.
- Using the previous two columns, make three new visualizations, choosing from `mark_area()`, `mark_bar()`, `mark_circle()`, `mark_line()`, `mark_rect()`, `mark_rule()`, `mark_square()`, `mark_text()`, `mark_tick()`. For each one, describe a pro and con to using this graph to visualize the data. For each one, also write a comment of what this type of graph allowed you to observe about the data.
- Make another visualization, choosing from `mark_area()`, `mark_bar()`, `mark_circle()`, `mark_line()`, `mark_rect()`, `mark_rule()`, `mark_square()`, `mark_text()`, `mark_tick()`, where you transform the data (such as bins, averages, etc). Write a comment of what you observe about the data.

## Bonus Challenge:

Find an example visualization from the Altair Example Gallery (<https://altair-viz.github.io/gallery/>), and copy the code into your own notebook, and get it to work with your data source (the COVID dataset).

## Resources

<https://uwdata.github.io/visualization-curriculum/altair_introduction.html>

## Tips and Suggestions

When making your graphs, do not try to do everything at once. First make sure the data is showing on the graphs, then start adding other elements/parameters.

## Deadlines and Deliverables

The deliverable should be committed and pushed to the main branch of your repository on GitHub. It is due Monday, March 31st. Your notebook file (i.e. `.ipynb`) file should be committed and pushed to your homework repository, along with other necessary files such as `pyproject.toml`, `uv.lock`, and `README.md`.
