# SH Automation Ninjas - Training Syllabus

Welcome to the training syllabus for SH Automation Ninjas. This document outlines the topics covered in our six training sessions. Each session will delve into an exercise that will help us familiarize ourselves with Google Apps Scripts, APIs, and automating tasks with the help of ChatGPT.

## Session 1 - Remove Duplicates and Organize Data

In our first session, we'll work on a task involving a Google Sheet with three tabs. Our objective will be to create a script that removes duplicate entries from a 'New Leads' list when compared against a 'Master Contact List', and then copies the unique new leads over to a third 'Output' tab.

For this session, make a copy of this set of data as your [test data](https://docs.google.com/spreadsheets/d/1EBSwlbsk6yZd100NH0e4wpd4o07ZELXYLTMrYDv9reY/edit#gid=1552392585)

*Learning Objective: Understand the basics of Google Apps Script and how to generate scripts with ChatGPT. Learn to automate simple data operations in Google Sheets.*

## Session 2 - API Calls and Data Retrieval

In the second session, we'll learn about APIs and how to call them to retrieve data. A Web API is like a waiter in a restaurant. You (the app) give it your order (request), it takes that to the kitchen (the web server), and brings back your food (data or service). It helps different software talk to each other over the internet.

Our task will involve calling our company's API to retrieve transactions for a particular period. We'll then identify the most frequent customers from this data and organize this information in a Google Sheet.

To get your API key, go to this [link](https://internal.shub.us/), click New Ticket and select "retrieve api key" on the drop down list. Input the login email for your employee test account and your api key will be emailed to you. 

For this session, we will be using the API documented in this [Google Doc](https://docs.google.com/document/d/1gVGpmTB-8m_VfrcUY1LxRu7KTkk2Duxi5ltRyJyHNhE/edit).

*Learning Objective: Learn about APIs, how to make API calls from Google Apps Script, and how to process the returned data. Expand on your knowledge of Google Apps Script.*

## Session 3 - Building a HTML Interface and Using Triggers

The third session will build upon our Google Apps Script knowledge. We will create a HTML interface that provides a summary of data, including most frequent customer, most recent visit, and amount spent in the period. We'll also learn how to use this interface to submit data to our sheet. Additionally, we'll cover using triggers within Google Apps Script to update the extracted data periodically.

We start from what we've done in the previous session, which was to extract transactions in the last 7 days. What we would notice is that the customer name is not available in the transactions data. Instead, a customer ID is provided. So now, we would want to call our SH API, to get customer, which would return our full customer list. 

Then we tell ChatGPT what columns we have on each sheet, and tell GPT that we want to have a HTML page that summarises Customer name, number of visits in last 7 days, and total spent. We also tell GPT that we want to add an additional column on the customer page, where we want to be able to submit a voucher for a customer using the HTML page. We will indicate this by typing in the customer name and hitting submit. GPT will need to generate a random 8 digit voucher code.

*Learning Objective: Learn how to build a HTML interface, interact with Google Sheets data from this interface, and create periodic triggers to automate tasks.*

## Session 4 - Communicating with ChatGPT, Code Efficiency, and Using Logger

In our fourth session, we'll focus on learning how to effectively communicate with ChatGPT to troubleshoot code. We'll discuss how to phrase our prompts to get the best assistance from the AI. We'll also dive into ways to improve the efficiency of our code, learning how to optimize our scripts for better performance.

A significant portion of this session will be devoted to using Google Apps Script's Logger class to identify and debug erroneous behavior or breaks in the code. We will learn how to log information in our scripts, how to view these logs, and how to use this information to debug our code.

*Learning Objective: Learn how to effectively communicate with ChatGPT for troubleshooting, how to improve code efficiency, and how to use the Logger class in Google Apps Script to debug scripts.*

## Session 5 - Integrating and Cross-Referencing Data from Different APIs

Our fifth session will level up the complexity slightly. We'll work with two APIs - one for transactions, and another for product inventory. We'll call both APIs, identify the top-selling products from the transactions, cross-reference this data with the inventory status of these products, and visualize the final data in a Google Sheet.

*Learning Objective: Learn how to work with multiple APIs and cross-reference data from different sources. Gain proficiency in data processing and visualization within Google Sheets.*

## Session 6 - Building a Complete Automation Scenario

In our final session, we will take a real-world automation scenario. The specifics of this session are to be decided, but it will integrate all the knowledge and skills we have accumulated in the previous sessions. 

*Learning Objective: Implement a complex real-world task that involves elements learned in previous sessions, and understand how these elements come together in a practical application.*

Remember, the main objective of these exercises is not just to create the scripts, but to learn how to generate scripts using ChatGPT,
