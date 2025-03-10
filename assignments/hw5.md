---
layout: page
title: HW05 Hypothesis
permalink: assignments/hw5
parent: Assignments
---

# Homework 5 **Due Monday Mar 17th at 2pm EDT**{: .label .label-red }

In this homework, you will use Hypothesis, a property-based testing tool, to find an obscure-ish bug in Wordle.

Please read the entire assignment in full before you begin. You might find some helpful information in the [Resources](#resources) section.

## Learning goals

- Think of a property that should always hold for function `is_yellow`
- Describe the property in your own words
- Use Hypothesis to implement your property test for `is_yellow`
- Find an obscure Wordle bug using Hypothesis

## Tasks

For this assignment, you will test a buggy version of Wordle using Hypothesis and try to find a bug.

You will perform the following tasks. You can use Codespaces for this assignment.

- Install Hypothesis
- Define your `is_yellow` property in your own words
- Implement your property in `wordle_parts_test.py`
- Find the bug using Hypothesis
- Bonus Challenge: Fix the bug!

### Create homework repo via GitHub Classroom

Your first step for this project is to create your repository that you will be working in for this assignment. You should create a repository via GitHub Classroom using this link: <https://classroom.github.com/a/IP-I2JCx> After accepting the homework, GitHub Classroom will create a repo named `cmu-crafting-software/2025-homework05-$YOUR_GITHUB_ID`.

You'll need to install a couple packages. To do so, use [uv](https://docs.astral.sh/uv/):

```sh
uv init
uv add hypothesis pytest
```

When you run these commands, VS Code should ask if you want to activate the virtual environment in the `.venv` folder that uv just created; click **Yes**. (Also, if any of the above terminal commands don't work, run the VS Code **Codespaces: Rebuild Container** command and then try again.)

Please also create a `README.md` file with the following information:

- The title of the homework (`# Homework 5`)
- Your name and Andrew ID

### Define your `is_yellow` property in your own words

Think about the cases when `is_yellow` should return true and when it should return false. Without re-implementing `is_yellow` can you think of some ways to predict when `is_yellow` might return true and when it might return false?

This may take some time and creativity. Write the property you choose in your own words in `README.md`.

### Implement your property in `wordle_parts_test.py`

Write a short test in function `test_is_yellow_pbt` that you think might find the bug.

> **Note**: Short here means under 10 lines of code; if writing more than that you may want to consider a simpler property.

### Find the bug using Hypothesis

To execute Hypothesis, run `uv run pytest` in your terminal.

If all tests pass, Hypothesis will say the tests passed (meaning it didn't find the bug). If a test fails, Hypothesis will show you a single example as well as the assertion that failed. The documentation (see Resources) also explains this.

When you find the bug, update `README.md` with:

- The counter-example Hypothesis found.
- A description of your experience trying to find the bug. Do you think this might be harder or easier than manually thinking of test cases?
- Anything that you liked or disliked about using Hypothesis. How do you think it could be better or easier to use?

> **Note**: If your property didn't find a bug, you should consider other properties to test.

## Bonus Challenge: Fix the Bug!

Correct the bug: include a corrected version of Wordle in your repo named `wordle_parts_fixed.py`

## Resources

- Hypothesis Documentation: <https://hypothesis.readthedocs.io/>
- Hypothesis Quick Start Guide: <https://hypothesis.readthedocs.io/en/latest/quickstart.html>
- Getting Started With Property-Based Testing in Python: <https://semaphoreci.com/blog/property-based-testing-python-hypothesis-pytest>
- Testing your Python Code with Hypothesis: <https://www.inspiredpython.com/course/testing-with-hypothesis/testing-your-python-code-with-hypothesis>

## Tips and Suggestions

You can assume that `is_green` and `is_red` are correctly implemented. If you get completely stuck, consider whether any position may ever be anything other than red, green, or yellow.

## Deadlines and Deliverables

**Due Date**: Monday March 17th at 2pm EDT

The deliverable should be committed and pushed to the main branch of your repository on GitHub.
