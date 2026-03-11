# Group Expense Management System (AWS Serverless)

## Overview

The **Group Expense Management System** is a serverless cloud-based application designed to simplify the process of managing shared expenses among groups. Whether it is a trip, shared accommodation, or group activity, tracking who paid and who owes money can be complicated.

This project provides a simple web-based solution where users can create groups, add expenses, and automatically split the costs among members. The system is built using **AWS serverless services**, allowing the application to scale efficiently without managing servers.

---

## Problem Statement

Managing group expenses manually often leads to:

* Calculation errors
* Confusion about who paid and who owes money
* Lack of a centralized place to track expenses

This project solves the problem by providing a **cloud-based automated expense tracking system** that records expenses, calculates splits automatically, and stores data securely. 

---

## Architecture

The application follows a **serverless architecture** using AWS services:

* **Amazon S3** – Hosts the static frontend website
* **Amazon API Gateway** – Provides REST API endpoints
* **AWS Lambda** – Handles backend logic for expense processing
* **Amazon DynamoDB** – Stores expense records and user data

---

## System Workflow

1. The user opens the web application hosted on **Amazon S3**.
2. The user adds an expense through the interface.
3. The frontend sends a request to **API Gateway**.
4. API Gateway triggers an **AWS Lambda function**.
5. Lambda processes the expense, calculates the split, and stores it in **DynamoDB**.
6. The system returns the updated expense data to the user.

---

## Features

* Create and manage expense groups
* Add and track shared expenses
* Automatically split expenses among members
* Store expense records in a cloud database
* Scalable and serverless architecture

---

## Technologies Used

* AWS Lambda
* Amazon API Gateway
* Amazon DynamoDB
* Amazon S3
* Python
* JavaScript / HTML / CSS (Frontend)

---

## Project Structure

```
group-expense-management-serverless
│
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── app.js
│
├── lambda-function/
│   └── expense_splitter.py
│
├── architecture/
│   └── architecture-diagram.png
│
└── README.md
```

---

## Learning Outcomes

Through this project, I learned:

* Designing **serverless applications using AWS**
* Building **REST APIs with API Gateway**
* Implementing backend logic with **AWS Lambda**
* Managing cloud databases using **DynamoDB**
* Hosting web applications using **Amazon S3**

---

## Future Improvements

* Add user authentication using **AWS Cognito**
* Implement real-time notifications
* Improve UI with a modern frontend framework
* Add analytics for expense tracking

---

## Author

Divya A
Third Year AIML Student
Interested in Cloud Computing, AI, and Data Science
