# SH Automation Ninjas - Training Syllabus

Welcome to the training syllabus for SH Automation Ninjas. This document outlines the topics covered in our six training sessions. Each session will delve into an exercise that will help us familiarize ourselves with Google Apps Scripts, APIs, and automating tasks with the help of ChatGPT.

## Session 1 - Remove Duplicates and Organize Data

In our first session, we'll work on a task involving a Google Sheet with three tabs. Our objective will be to create a script that removes duplicate emails from a 'New Leads' list when compared against a 'Master Contact List', and then copies the unique new leads over to a third 'Output' tab.

For this session, make a copy of this set of data as your [test data](https://docs.google.com/spreadsheets/d/1EBSwlbsk6yZd100NH0e4wpd4o07ZELXYLTMrYDv9reY/edit#gid=1552392585)

*Learning Objective: Understand the basics of Google Apps Script and how to generate scripts with ChatGPT. Learn to automate simple data operations in Google Sheets.*

## Session 2 - Communicating with ChatGPT, Code Efficiency, Understanding Functions, and Using Logger

In our second session, we'll focus on learning how to effectively communicate with ChatGPT to troubleshoot and generate code. We'll discuss how to phrase our prompts to get the best assistance from the AI. We'll also dive into ways to improve the efficiency of our code, learning how to optimize our scripts for better performance.

This session will introduce the concept of functions, which are reusable blocks of code that perform a specific task. Functions can be combined to build more complex features, enhancing the modularity and readability of your code.

A significant portion of this session will be devoted to using Google Apps Script's Logger class to identify and debug erroneous behavior or breaks in the code. We will learn how to log information in our scripts, how to view these logs, and how to use this information to debug our code.

*Learning Objective: Learn how to effectively communicate with ChatGPT for troubleshooting and code generation. Understand the concept of functions and how they can be used to build complex features. Learn how to improve code efficiency, and how to use the Logger class in Google Apps Script to debug scripts.*

## Session 3 - API Calls and Data Retrieval

In the third session, we'll learn about APIs and how to call them to retrieve data. A Web API is like a waiter in a restaurant. You (the app) give it your order (request), it takes that to the kitchen (the web server), and brings back your food (data or service). It helps different software talk to each other over the internet.

Our task will involve calling our company's API to retrieve transactions for a particular period. We'll then identify the most frequent customers from this data and organize this information in a Google Sheet.

To get your API key, go to this [link](https://internal.shub.us/), click New Ticket and select "retrieve api key" on the drop down list. Input the login email for your employee test account and your api key will be emailed to you. 

For this session, we will be using the API documented in this [Google Doc](https://docs.google.com/document/d/1gVGpmTB-8m_VfrcUY1LxRu7KTkk2Duxi5ltRyJyHNhE/edit).

*Learning Objective: Learn about APIs, how to make API calls from Google Apps Script, and how to process the returned data. Expand on your knowledge of Google Apps Script.*

## Session 4 - Building a HTML Interface and Using Triggers

Our fourth session extends our Google Apps Script skill set and dives into user interface creation with HTML. In this session, we will build a user-friendly HTML interface that displays a summary of key customer data, including the customer's name, their number of visits in the last seven days, and their total spend during that period. Furthermore, we'll learn how to use this interface to submit data to our Google Sheet, adding an exciting interactive component to our work.

In addition to UI creation, we'll explore how to use triggers within Google Apps Script. Triggers let us automate tasks and periodically update the extracted data without manual intervention. This hands-off approach ensures our data stays current and relevant.

Building upon our previous session's work, we'll use transaction data from the last seven days. As we've previously noticed, the transactions data includes a customer ID but not the customer's name. To obtain the names, we'll call the SH API, which provides us with our full customer list. 

We will then engage with ChatGPT, providing the columns we have on each sheet and specifying our desired outcome: a HTML page summarising customer data and a new column in the customer sheet. This new column, manipulated through our HTML page, will allow us to submit a voucher for a customer by typing in their name and clicking submit. ChatGPT will generate a random eight-digit voucher code, further personalising the customer experience.

*Learning Objective: Acquire skills in building a HTML interface and interacting with Google Sheets data from this interface. Learn to create periodic triggers to automate tasks. Understand the role of unique customer identifiers and the generation of randomised voucher codes.*

## Session 5 - Integrating and Cross-Referencing Data from Different APIs

Our fifth session will level up the complexity slightly. We'll work with two APIs - one for transactions, and another for product inventory. We'll call both APIs, identify the top-selling products from the transactions, cross-reference this data with the inventory status of these products, and visualize the final data in a Google Sheet.

*Learning Objective: Learn how to work with multiple APIs and cross-reference data from different sources. Gain proficiency in data processing and visualization within Google Sheets.*

## Session 6 - Building a Complete Automation Scenario

In our final session, we will take a real-world automation scenario. The specifics of this session are to be decided, but it will integrate all the knowledge and skills we have accumulated in the previous sessions. 

*Learning Objective: Implement a complex real-world task that involves elements learned in previous sessions, and understand how these elements come together in a practical application.*

Remember, the main objective of these exercises is not just to create the scripts, but to learn how to generate scripts using ChatGPT.
