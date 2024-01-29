---
layout: page
title: HW01  Version Control
permalink: /assignments/hw1
parent: Assignments
---

# Homework 1 **Due Friday Feb 2nd at 4pm EST**{: .label .label-red }
In this homework, you will be practicing using version control (`git` and [GitHub](https://github.com/)). We will be using this throughout the course extensively.  Additionally, we will be requiring you to use the command line for this assignment. 


## Learning goals
- Understand basic concepts of Version Control Systems (VCS)
- Create Github Account
- Performing basic VCS actions
- Understand difference between `git` and GitHub
- Practice VCS commands necessary for turning in homeworks

## Tasks
You will be asked to perform the following series of tasks:
- Create a GitHub account
- Clone HW1 repo
- Create a branch locally
- Learn to manage conflicts
- Push branch to github
- Make a change to the student list
- Open a Pull Request to the `main` branch


### Create a Github account
You should create a free [GitHub](https://www.github.com) account if you do not already have one.  If you are creating a new GitHub account, you might want to consider using your andrewID, as that will make things easier for us.  But you may use any account name you want.
If you have an existing GitHub account, you may use that.

### Clone HW1 repo
There is a very simple repo that has been setup for HW1. You can find it [here](https://github.com/cmu-crafting-software/Homework01).  You should clone the repo to a local directory on your machine.   This should be done via the command line, and you should include the command(s) needed in your script to turn in.

### Create a branch locally
You should create a new branch of the repository, and you should name the branch with your andrewID as the name.  This should be done via the command line, and you should include the command(s) needed in your script to turn in.


### Make a change to the student list, commit locally, and managing any conflicts that might exist
In the branch that you created, you should make a change to the `ClassRoster.md` file, adding your name and andrewID to the Class Roster.  You should then commit that change to your local branch.  Commiting should be done via the command line, and you should include the command(s) needed in your script to turn in.


### Push branch to github
Once you have committed your change, you should push the change on the branch to the GitHub repository.  Please ensure you use a descriptive commit message! This should be done via the command line, and you should include the command(s) needed in your script to turn in.


### Open a Pull request to the main branch
Now that the commit is visible on the GitHub site, you should open a Pull Request from your personal branch, to the main branch.  Again, don't forget to have a descriptive message for the Pull Request.  You do not need to do this via the command line, you may use the GitHub website for opening the pull request.

### Manage merge conflicts 
Merge conflicts can be very annoying, and will be a cause of headaches for you.  We want you to try and follow these steps to (artificially) create a merge conflict, so that you can merge the conflict. Here are the steps to follow:
- In the branch < andrewID >, create a text file called `student_facts.txt`
- In this file, write what year and college you are in
- Commit this change and include a message about what you just did
- Create a new branch called < new_andrewID > and switch to that branch
- Open up `student_facts.txt` and delete the previous line you wrote and now only include a sentence about a fun fact about yourself
- Commit this change and include a message about what you just did
- Switch back to the branch < andrewID >
- Open up `student_facts.txt` and append to this file a sentence about what programming languages and/or coding classes you have taken
- Commit this change and include a message about what you just did
- While in < andrewID >, merge this branch with < new_andrewID >
- You will see that there are conflicts
- To resolve these conflicts, open on the file `student_facts.txt` and edit the file such that there are three different lines with (and in this order):
  - A sentence about your year and major
  - A sentence about what programming languages and/or coding classes you have taken
  - A sentence with a fun fact about yourself
  - Commit this change and include a message about what you just did
- While in < andrewID >, create a file with all of the Terminal commands you used so far
The appropriate steps here should be done via the command line, and you should include the command(s) needed in your script to turn in.



## Resources
1. <https://guides.github.com/>
2. <https://guides.github.com/activities/hello-world/>
3. <https://docs.github.com/en/desktop/installing-and-configuring-github-desktop/getting-started-with-github-desktop>
4. <https://gist.github.com/davfre/8313299>
5. <https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository>


## Tips and Suggestions
We are requiring you to learn to use the command line interface for this assignment.  While there are several `git` clients ([SourceTree](https://www.sourcetreeapp.com/), [Github Desktop](https://desktop.github.com/)) available, and if you find yourself struggling, you might want to try using a client first, then re-doing the assignment with the command line. 

Writing a good commit message is hard! Don't feel bad if it takes a bit of thinking, or if you are not happy with your first version.

One pro tip with `git`.  It can often be the case that your local directory can get really messed up. Feel free to delete your local directly and start over.  This is a common technique when working with `git`.

## Deadlines and Deliverables
__Due Date__: Friday Feb 2nd at 4pm.  
You may use up to two (2) late days, out of six total.  To use a late day, simply message us on slack to let us know that you will be using a late day.

__Deliverable__: For this assignment, you have two deliverables.  
You will turn in a script that shows what commands you used at the command line. You should turn this in by sending it to both instructors and the TA in a group message via slack. 
Your commits to the repository will be viewable by us, and we will use them for grading (you might want to confirm that they are visible by using the GitHub web interface).



## Assignment Review
Because this is a new class, we are asking you to fill out a short survey to help us calibrate the homeworks.  This survey is ungraded, but your input will be very valuable for us in improving the course both for this semester, and for future years. [__Fill out a short survey to help us improve the course!__](https://forms.gle/z3i3o2V8GWsvDYzJ9)

