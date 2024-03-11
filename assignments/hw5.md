---
layout: page
title: HW05 Hypothesis
permalink: /assignments/hw5
parent: Assignments
---

# Homework 5

**Due Friday Mar 15th at 4:00pm EST**{: .label .label-red } 

In this homework, you will use Hypothesis, a property-based testing tool, to find an obscure-ish bug in Wordle. 

Please read the entire assignment in full before you begin. You might find some helpful information in the [Resources](#resources) section.

## Learning goals

- Think of a property that should always hold for function `is_yellow`. 
- Describe the property in your own words
- Use Hypothesis to implement your property test for `is_yellow`
- Find an obscure Wordle bug using Hypothesis

## Tasks

For this assignment, you will test a buggy version of Wordle using Hypothesis and try to find a bug.

You will perform the following tasks. You can use Codespaces for this assignment.

- Install Hypothesis
- Setup your `hw5` folder
- Define your `is_yellow` property in your own words
- Implement your property in `wordle_parts_test.py`
- Find the bug using Hypothesis
- Bonus Challenge: Fix the bug!

### Install Hypothesis

Using the terminal in your homework repo:

```
pip install hypothesis
```

### Setup your `hw5` folder

1. In your homework repo:
   ```
   mkdir hw5
   cd hw5
   ```
2. Dowload the following files into `hw5`:
   - Buggy Wordle: `wordle_parts_buggy.py` <https://gist.githubusercontent.com/cmumatt/d8973817349b243a88b034c654c7fda9/raw/c4ecd84b4c2c6119ea70ef13e70c69b595361093/wordle_parts_buggy.py>
   - Starter test code: `wordle_parts_test.py` <https://gist.githubusercontent.com/cmumatt/75fbf9d12b703a2021666db38adc3123/raw/912127dad10aca9796f00110173a227ff04dfc2f/wordle_parts_test.py>
3. Create a blank `README.md` in `hw5`
4. Stage, commit, and push to the remote repository

### Define your `is_yellow` property in your own words

Think about the cases when `is_yellow` should return true and when it should return false. Without re-implementing `is_yellow` can you think of some ways to predict when `is_yellow` might return true and when it might return false?

This may take some time and creativity. Write the property you choose in your own words in `README.md`.

### Implement your property in `wordle_parts_test.py`

Write a short test in function `test_is_yellow_pbt` that you think might find the bug. 

> **Note**: Short here means under 10 lines of code; if writing more than that you may want to consider a simpler property.

### Find the bug using Hypothesis

To execute Hypothesis, run `pytest` in terminal with `hw5` as your current working directory.

If all tests pass, Hypothesis will say the tests passed (meaning it didn't find the bug). If a test fails, Hypothesis will show you a single example as well as the assertion that failed. The documentation (see Resources) also explains this.

When you find the bug, update `README.md` with the counter-example Hypothesis found and describe your experience and how easy or hard it was to find the bug versus how hard you think it might have been to find the bug by manually thinking of test cases.

> **Note**: If your property didn't find a bug, you should consider other properties to test.

## Bonus Challenge: Fix the Bug! 

Correct the bug in `wordle_parts_buggy.py` and include a corrected version in your repo named `wordle_parts_fixed.py`

## Resources

* Hypothesis Documentation: <https://hypothesis.readthedocs.io/>
* Hypothesis Quick Start Guide: <https://hypothesis.readthedocs.io/en/latest/quickstart.html>
* Getting Started With Property-Based Testing in Python: <https://semaphoreci.com/blog/property-based-testing-python-hypothesis-pytest>
* Testing your Python Code with Hypothesis: <https://www.inspiredpython.com/course/testing-with-hypothesis/testing-your-python-code-with-hypothesis>

## Tips and Suggestions

You can assume that `is_green` and `is_red` are correctly implemented. If you get completely stuck, consider whether any position may ever be anything other than red, green, or yellow.

## Deadlines and Deliverables

__Due Date__: Friday March 15th at 4:00pm EST

The deliverable should be committed and pushed to the main branch of your repository on GitHub inside a `hw5` subdirectory.
