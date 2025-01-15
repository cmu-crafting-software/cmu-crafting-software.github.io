---
layout: page
title: HW02  Reading Data
permalink: /assignments/hw2
parent: Assignments
published: false
---

# Homework 2 **Due Tuesday Feb 9th at 4pm EST**{: .label .label-red }
In this homework you will practice writing a Python application, as well as reading data from various sources. Please read the entire assignment in full before you begin. You might find some helpful information in the Resources section. 

## Learning goals

- Run Python application
- Read in data from a CSV file
- Store data in the application 
- Calculate some basic statistics from data collected

## Tasks

You will be asked to perform the following series of tasks:

- Clone the homework repo via GitHub Classroom.
- Read csv file of weather forecast data
- Print weather data
- Calculate the average, minimum, and maximum of the `temperature` column in the data set
- Read data directly from the US National Weather Service using their API
- Show correctness by confirming the data on the website and calculating `temperature` again

### Clone Homework Repo via GitHub Classroom.

Your first step for this project is to configure your repository that you will be working in for this assignment. You should create a repository via Github classroom at this link: <https://classroom.github.com/a/N2lGzl0s>. After accepting the homework, GitHub classroom will create a repo named `crafting-software-hw-<your-github-id>`. We will use this repo for future assignments, too.

You will be committing your solutions to the `hw2` folder in this repo for all this homework.

### Read `.csv` file of weather data

You should write a small program in Python that will read data from the `weather.csv` file. You can find the CSV file in your cloned repo, which include weather forecast data for Pittsburgh, PA on Jan 24, 2022.

Then, you should write a small program to read each line of `weather.csv` into your program.

You should push a commit to your repository with a descriptive commit message once you have reached this point.

### Print weather data

The next step is to simply print out the data using the `print` function in your application. Once you have achieved this, you should commit this change to your repository, and push it to your repo.

### Calculate the average, min, and max of the `temperature` column in the data set

The data in the `.csv` is documented by the first row in the dataset. You should  calculate the average, max, and min of the `temperature` column in the file.

To confirm these are the correct values, you should import the `.csv` file into a spreadsheet (Excel, Google Sheets, etc), and calculate the same values, and compare them.  You should then commit this code. In the commit message and the `hw2/README` page, you should specify what the values were.

### Read data directly from the National Weather Service API

Another way to get the data from National Weather Service is to use their API (Application Programming Interface). You can find the API documented here: <https://www.weather.gov/documentation/services-web-api>. This time, you will get the most recent forecast data for Pittsburgh, PA.

To get the data from the API, you will need to make a request.  To make the API call, you should use the `requests` Python library: <https://requests.readthedocs.io/en/master/>.

**NOTE:** installing requests might go smoothly, or it might be difficult. Please don’t hesitate to reach out, as there are lots of small things that could make this step go wrong.

To confirm that you have retrieved the data, you should print it out. Then, you should commit and push this to your homework repository.

### Show correctness by calculating a value available on the website, to confirm correctness

To verify that you are using the data correctly, you can find the most recent forecast information on the National Weather Service website: <https://www.weather.gov/forecastmaps>.

Just like the last time with `weather.csv`, you should calculate the min, max, and average of the temperature and compare it against the value on the site. Your commit message should show what the value is, and what confirm what your calculated value is.

## Resources

Some Resources that might be helpful: 

Running Python code in virtual env:
* <https://docs.python.org/3/tutorial/venv.html>

Reading a csv in Python: 
* <https://realpython.com/python-csv/>
* <https://stackoverflow.com/questions/11310248/find-number-of-columns-in-csv-file>
* <https://docs.python-guide.org/starting/install3/osx/>

Pip installing requests: 
* <https://requests.readthedocs.io/en/master/user/install/>
* <https://stackoverflow.com/questions/18363022/importerror-no-module-named-pip>

Using requests: 
* <https://realpython.com/python-requests/>
* <https://stackoverflow.com/questions/31126596/saving-response-from-requests-to-file>
* <https://learning.postman.com/docs/sending-requests/requests/#creating-requests>


## Tips and Suggestions

* If you copy code from the internet, add a comment to attribute it.
* The National Weather Service API doesn't accept locations like `Pittsburgh, PA` as an input. To find out what format it requires, read their [FAQ page](https://weather-gov.github.io/api/general-faqs). 
  * There are many tools online (e.g. Google Maps) that converts from city names to coordinates.

## Deadlines and Deliverables
__Due Date__: Tuesday Feb 9th at 4pm.  

You may use up to two (2) late days, out of six total.  To use a late day, simply message us on slack to let us know that you will be using a late day.

__Deliverable__: For this assignment, you have one deliverable.

You should commit the code you have written to your repository as you go along. Your `hw2/README.md` file should also contain description of what's in the repo and the results of data analysis in this homework.

When you are ready to submit, you should create a new tag, your tag should be `2.0` (for HW2). (<https://git-scm.com/book/en/v2/Git-Basics-Tagging>) then send a group message to the instructors and TA via Slack.

## Assignment Review

Because this is a new class, we are asking you to fill out a short survey to help us calibrate the homeworks.  This survey is ungraded, but your input will be very valuable for us in improving the course both for this semester, and for future years. [__Fill out a short survey to help us improve the course!__](https://forms.gle/z3i3o2V8GWsvDYzJ9)
