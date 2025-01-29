---
layout: page
title: HW02 Reading Data
permalink: /assignments/hw2
parent: Assignments
---

# Homework 2 **Due Friday Feb 7th at 2pm EST**{: .label .label-red }
In this homework you will practice writing a Python application, as well as reading data from various sources. Please read the entire assignment in full before you begin. You might find some helpful information in the Resources section. 

## Learning goals

- Run Python application
- Read in data from a CSV file
- Store data in the application 
- Calculate some basic statistics from data collected

## Tasks

You will be asked to perform the following series of tasks:

- Open the homework repo in GitHub Codespaces.
- Read the CSV file of weather forecast data.
- Print the weather data.
- Calculate the average, minimum, and maximum of the `temperature` column in the data set.
- Read data directly from the US National Weather Service using their API.
- Show correctness by confirming the data on the website and calculating `temperature` again.

### Open homework repo in GitHub Codespaces

Your first step for this project is to open a Codespace in repository that you will be working in for this assignment: <https://github.com/cmu-crafting-software/homework02>

Create and switch to a new branch whose name is your Andrew ID, and push it to the repository.

### Read CSV file of weather data

You can find the CSV file in the repo, which include weather forecast data for Pittsburgh, PA on Jan 24, 2022. You should write a small program to read each line of `weather.csv` into your program. Push a commit to the repository with a descriptive commit message once you have reached this point.

### Print weather data

The next step is to simply print out the data using the `print` function in your application. Once you have achieved this, you should commit this change to the repository, and push it to GitHub.

### Calculate average, min, and max of the `temperature` column in the data set

The data in `weather.csv` is documented by the first row in the dataset. You should calculate the average, max, and min of the `temperature` column in the file.

To confirm these are the correct values, you should import `weather.csv` file into a spreadsheet (Excel, Google Sheets, etc), and calculate the same values, and compare them. You should then commit this code. In the commit message and in `README.md`, you should specify what the values were.

### Read data directly from the National Weather Service API

Another way to get the data from National Weather Service is to use their API (Application Programming Interface). You can find the API documented here: <https://www.weather.gov/documentation/services-web-api>. This time, you will get the most recent forecast data for Pittsburgh, PA.

To get the data from the API, you will need to make a request. To make the API call, you should use the `requests` Python library, which comes preinstalled in GitHub Codespaces: <https://requests.readthedocs.io/en/master/>.

To confirm that you have retrieved the data, you should print it out. Then, you should commit and push this to the homework repository.

### Show correctness by calculating a value available on the website, to confirm correctness

To verify that you are using the data correctly, you can find the most recent forecast information on the National Weather Service website: <https://www.weather.gov/forecastmaps>.

Just like the last time with `weather.csv`, you should calculate the min, max, and average of the temperature and compare it against the value on the site. Your commit message should show what the value is, and what confirm what your calculated value is.

## Resources

Some Resources that might be helpful: 

Reading a CSV file in Python: 
* <https://realpython.com/python-csv/>
* <https://stackoverflow.com/questions/11310248/find-number-of-columns-in-csv-file>
* <https://docs.python-guide.org/starting/install3/osx/>

Using `requests`: 
* <https://realpython.com/python-requests/>
* <https://stackoverflow.com/questions/31126596/saving-response-from-requests-to-file>
* <https://learning.postman.com/docs/sending-requests/requests/#creating-requests>


## Tips and Suggestions

* If you copy code from the internet, add a comment to attribute it.
* The National Weather Service API doesn't accept locations like `Pittsburgh, PA` as an input. To find out what format it requires, read their [FAQ page](https://weather-gov.github.io/api/general-faqs). 
  * There are many tools online (e.g. Google Maps) that converts from city names to coordinates.

## Deadlines and Deliverables

**Due Date**: Friday Feb 7th at 2pm.

You may use up to two (2) late days, out of six total. To use a late day, simply message us on Slack to let us know that you will be using a late day.

**Deliverable**: For this assignment, you have one deliverable.

You should commit the code you have written to your branch in the repository as you go along. Your `README.md` file should also contain description of what's in the repo and the results of data analysis in this homework.

When you are ready to submit, send a group message to the instructors and TA via Slack.

## Assignment Review

Because this is a new class, we are asking you to fill out a short survey to help us calibrate the homeworks.  This survey is ungraded, but your input will be very valuable for us in improving the course both for this semester, and for future years. [**Fill out a short survey to help us improve the course!**](https://forms.gle/FuStF6Xr1Q7hvW3a8)
