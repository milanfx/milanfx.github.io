---
layout: page
title: /M1C1/
permalink: /M1C1/
---

### M4Lab1 - Implement AI-assisted SQL Queries

#### 🗂️ Overview

In this activity, you will engage in a hands-on experience using GitHub Copilot by Microsoft to create and optimize SQL queries. This interactive exercise is designed to demonstrate how generative AI can assist in making SQL query writing more efficient and effective. By comparing AI-generated queries to manually written ones, you will gain insight into the capabilities and efficiency of using AI tools in SQL database management.

#### 🗂️ Learning Outcomes

- Implement AI-assisted SQL Queries

---

#### 🗂️ Task 1: Basic Query Generation with Copilot

Objective: Formulate a query retrieving track names for all tracks in the Track table where the genre is ‘Rock’.

✅️ Step 1: Start with a SELECT statement and observe Copilot’s suggestions for completing your query.

✅️ Step 2: Compare the AI-generated query with your manually written attempt.

Tip: Pay attention to how Copilot suggests completing the query.

Test Your Work: Check if the query returns the expected track names for the ‘Rock’ genre.

```SQL
-- Task 1: Basic Query Completion with Copilot
SELECT NameFROM Track
WHERE GenreId = (
	SELECT GenerId
	FROM Genre
	WHERE Name = 'Rock'
);
```

---

#### 🗂️ Task 2: Applying Filtering and Sorting

✅️ Step 1: Copy the following starter code.

✅️ Step 2: Complete the SELECT statement on the Customer table using an alias.

✅️ Step 3: Create a JOIN on the Invoice table using an alias.

✅️ Step 4: Let Copilot assist in what columns to join.

✅️ Step 5: In the SELECT statement begin adding the columns and let Copilot assist with adding the columns and syntax.

✅️ Step 6: Then, let Copilot assist with optimizing the query by adding a WHERE clause to filter the results based on a specific condition, and the ORDER BY clause to sort the results.

✅️ Step 7: Analyze differences between the AI-generated and manual queries.

Tip: Notice how Copilot helps structure the query.

Test Your Work: Output should show the invoice details sorted by purchase date.

```SQL
-- Task 2: Applying Filters and Sorting
-- Create a SELECT statement on the Customer table using an alias.
SELECT
    c.FirstName AS CustomerFirstName,
    c.LastName AS CustomerLastName,
    i.InvoiceId,
    i.InvoiceDate,
    i.Total
-- Create a join with the Invoice table using an alias.
FROM
    Customer c
JOIN
    Invoice i ON c.CustomerId = i.CustomerId
WHERE i.Total > 10 
ORDER BY i.InvoiceDate DESC;

```

---

#### 🗂️ Task 3: Complex Query Optimization

✅️ Step 1: Copy the following starter code.

✅️ Step 2: Construct a manual query to list artists, albums, and their total sales figures in descending order. Use Copilot to make suggestions.

✅️ Step 3: Evaluate the AI-generated query for completeness and efficiency.

Tip: Check the efficiency of the AI-suggested query.

Test Your Work: Ensure the output correctly lists artist, albums, and their total sales figures in descending order.

```SQL
-- Task 3: Complex Query Optimization
SELECT
    ar.Name AS ArtistName,
    al.Title AS AlbumTitle,
    SUM(il.UnitPrice * il.Quantity) AS TotalSales
FROM Artist ar
JOIN Album al ON ar.ArtistId = al.ArtistId
JOIN Track t ON al.AlbumId = t.AlbumId
JOIN InvoiceLine il ON t.TrackId = il.TrackId
GROUP BY ar.Name, al.Title
ORDER BY TotalSales DESC;
```

#### 🗂️ Summary

Leveraging AI tools like GitHub Copilot by Microsoft can greatly enhance the efficiency and accuracy of SQL query writing. While AI can assist in generating and optimizing queries, it is important to validate and modify AI-generated code to fit specific needs accurately.


### Lab M2C4 - Sort Data in a Real-world Dataset

#### 🗂️ Overview

This hands-on activity empowers you to apply SQL skills in sorting and organizing data within a real-world dataset using the ORDER BY clause. By utilizing the Chinook Database, you will gain practical experience in applying sorting techniques essential for effective data organization and presentation.

#### 🗂️ Learning Outcomes

- Apply sorting techniques using the ORDER BY clause.
- Understand descending order and its uses. 
- Practice combined query techniques to achieve specific results. 

---

#### 🗂️ Task 1: Sort Customer Names

Objective: Practice ordering data alphabetically to improve data readability and navigation.

✅️ Step 1: Write a SQL query using the ORDER BY to retrieve and display customer names sorted alphabetically by their last names.

Tip: The default order is ascending, but it’s best practice to still include ASC in the code.

```SQL
-- Task 1: Sort Customer Names
-- Write a query to retrieve customer names sorted
-- alphabetically by their last names.
SELECT FirstName, LastName
FROM Customer
ORDER BY LastName ASC;
```

#### 🗂️ Task 2: Organize Tracks by Unit Price

Objective: Understand descending order and its role in financial analysis or resource prioritization.

✅️ Step 1: Formulate a query to retrieve the names of tracks sorted by their UnitPrice, from the most expensive to the least expensive.

Tip: To format in descending order, use the truncated DESC in your code. 

```SQL
-- Task 2: Organize Track by Unit Price
-- Write a query to retrieve the names of tracks sorted by their UnitPrice
-- in descending order, from the most expensive to the least expensive.
SELECT Name, UnitPrice
FROM Track
ORDER BY UnitPrice DESC;
```

#### 🗂️ Task 3: Combine Sorting with Filtering

Objective: Reinforce combined query techniques used to achieve specific results when sorting and filtering data.

✅️ Step 1: Using the following starter code, use a combination of WHERE and ORDER BY clauses to display InvoiceId for each CustomerId for customers in 'Germany', and ordered by Total in descending order.

```SQL
-- Task 3: Combine Sorting with Filtering
-- Retrieve the InvoiceId and CustomerId for customers located in 'Germany',
-- and sort the results by Total in descending order.
SELECT InvoiceId, CustomerId, Total
FROM Invoice
WHERE BillingCountry = 'Germany'
ORDER BY Total DESC;
```

#### 🗂️ Task 4: Multi-column Sorting

Objective: Learn to apply multi-level sorting, necessary for nuanced data analysis.

✅️ Step 1: Using the following starter code, construct a query to sort the tracks by MediaTypeId and, within each media type, by track name alphabetically.

```SQL
-- Task 4: Multi-column Sorting
-- Write a query to sort the tracks first by MediaTypeId in ascending order,
-- and then alphabetically by track name within each MediaTypeId.
SELECT Name, MediaTypeId
FROM Track
ORDER BY MediaTypeId ASC, Name ASC;
```

#### 🗂️ Summary

In this activity you explored advanced sorting techniques using the ORDER BY clause and ASC and DESC commands, enabling you to visualize your results in the most helpful way. Through practice, reflection, and feedback, you will strengthen your command over basic querying techniques essential for effective data manipulation.

### Topic 1: Data Movement Approaches
#### 1. Tools and processes:
- **Data movement approaches**
  - ETL
  - ELT
  - Data pipelines

### Topic 2: Extract, Transform, and Load Process
#### 1. ETL process:
- **ETL purpose**
  - Raw data converted into analysis-ready data
- **ETL nature**
  - Automated process
- **ETL steps**
  - Gather raw data from identified sources
  - Extract data aligned with reporting and analysis needs
  - Clean, standardize, and transform data
  - Load data into a data repository

#### 2. Extract:
- **Extraction methods**
  - Batch processing
  - Stream processing

#### 3. Batch processing:
- **Batch movement**
  - Source data moved in large chunks at scheduled intervals
- **Batch tools**
  - Stitch
  - Blendo

#### 4. Stream processing:
- **Real-time processing**
  - Data pulled and transformed in real time before loading
- **Stream tools**
  - Apache Samza
  - Apache Storm
  - Apache Kafka

#### 5. Transform:
- **Transformation rules**
  - Make date formats and units consistent
  - Remove duplicate data
  - Filter unnecessary data
  - Enrich data
  - Establish key relationships
  - Apply business rules and validations

#### 6. Load:
- **Load types**
  - Initial loading
  - Incremental loading
  - Full refresh
- **Load verification**
  - Data checks for missing or null values
  - Server performance monitoring
  - Load failure monitoring

#### 7. ETL usage:
- **Historical usage**
  - Batch workloads on a large scale
- **Streaming usage**
  - Real-time streaming event data

#### 8. ETL tools:
- **ETL tools**
  - IBM Infosphere Information Server
  - AWS Glue
  - Improvado
  - Skyvia
  - HEVO
  - Informatica PowerCenter

### Topic 3: Extract, Load, and Transform Process
#### 1. ELT process:
- **ELT sequence**
  - Data loaded before transformation
- **Transformation location**
  - Transformations applied in the target system

#### 2. ELT destination:
- **Target systems**
  - Data lake
  - Data warehouse

#### 3. ELT characteristics:
- **Technology basis**
  - Powered by cloud technologies

#### 4. ELT use cases:
- **Data types**
  - Large unstructured data
  - Non-relational data
- **Ideal environment**
  - Data lakes

#### 5. ELT advantages:
- **Shorter cycle**
  - No staging environment
- **Immediate ingestion**
  - Raw data ingested as available
- **Analytical flexibility**
  - Greater flexibility for exploratory analytics
- **Selective transformation**
  - Transform only data required for analysis
- **Big Data suitability**
  - More suited for Big Data

### Topic 4: Data Pipelines
#### 1. Data pipeline definition:
- **Pipeline scope**
  - Complete journey of data from one system to another

#### 2. ETL and ELT relationship:
- **Pipeline subsets**
  - ETL and ELT may be subsets

#### 3. Pipeline architectures:
- **Processing types**
  - Batch processing
  - Streaming data
  - Combined batch and streaming

#### 4. Streaming pipelines:
- **Continuous processing**
  - Data processed in continuous flow
- **Example use**
  - Sensor data monitoring traffic

#### 5. Pipeline performance:
- **Query support**
  - Long-running batch queries
  - Smaller interactive queries

#### 6. Pipeline destinations:
- **Target destinations**
  - Data lake
  - Applications
  - Visualization tools

#### 7. Pipeline solutions:
- **Pipeline tools**
  - Apache Beam
  - AirFlow
  - DataFlow







## ⭕️ C1 - Introduction to Data Engineering
### ✅️ M1 - What is Data Engineering?
#### ✔️ L1 - Course Introduction
- Video - Welcome to Introduction to Data Engineering


#### ✔️ L2 - Modern Data Ecosystem and role of Data Engineering
- Video - Modern Data Ecosystem 
- Video - Key Players  in the Data Ecosystem
- Video - Specializations in Data Engineering
- Video - What is Data Engineering?
- Video - Viewpoints: Defining Data Engineering
- Video - Viewpoints: Evolution of Data Engineering
- Read - Summary and Highlights
- Quiz - Practice Quiz
- Quiz - Graded Quiz


#### ✔️ L3 - Responsibilities and Skillsets of a Data Engineer
- Video - Responsibilities and Skillsets of a Data Engineer
- Video - Viewpoints: Skills and Qualities to be a Data Engineer
- Video - A Day in the Life of a Data Engineer
- Read - Summary and Highlights
- Quiz - Practice Quiz
- Quiz - Graded Quiz


### ✅️ M2 - The Data Engineering Ecosystem
#### ✔️ L1 - The Data Ecosystem and Languages for Data Professionals
- Video - Overview of the Data Engineering Ecosystem
- Video - Types of Data
- Video - Understanding Different Types of File Formats
- Video - Sources of Data
- Video - Languages for Data Professionals
- Video - Viewpoints: Working with Varied Data Sources and Types
- Read - Reading: Metadata and Metadata Management
- Read - Summary and Highlights
- Quiz - Practice Quiz
- Quiz - Graded Quiz


#### ✔️ L2 - Data Repositories, Data Pipelines, and Data Integration Platforms
- Video - Overview of Data Repositories
- Video - RDBMS
- Video - NoSQL
- Video - Data Warehouses, Data Marts, and Data Lakes
- Video - Data Lakehouses Explained
- Video - Viewpoints: Considerations for Choice of Data Repository
- Video - ETL, ELT, and Data Pipelines
- Video - Data Integration Platforms
- Video - Viewpoints: Tools, Databases, and Data Repositories of Choice
- Read - Summary and Highlights
- Quiz - Practice Quiz
- Quiz - Graded Quiz


#### ✔️ L3 - Big Data Platforms
- Video - Foundations of Big Data
- Video - Big Data Processing Tools: Hadoop, HDFS, Hive, and Spark
- Video - Viewpoints: Impact of Big Data on Data Engineering
- Read - Summary and Highlights
- Quiz - Practice Quiz
- Quiz - Graded Quiz


#### ✔️ L4 - Create an instance of IBM Db2 database
- Lab - Labs for IBM Cloud and Db2
- Lab - Obtain IBM Cloud Feature Code and Activate Trial Account
- Lab - Hands-on Lab: Create your IBM Cloud account
- Lab - Hands-on Lab: Provision an instance of IBM Db2 Lite plan


### ✅️ M3 - Data Engineering Lifecycle
#### ✔️ L1 - Data Platforms, Data Stores, and Security
- Video - Architecting the Data Platform
- Video - Factors for Selecting and Designing Data Stores
- Video - Security
- Video - Viewpoints: Importance of Data Security
- Read - Summary and Highlights
- Quiz - Practice Quiz
- Quiz - Graded Quiz


#### ✔️ L2 - Data Collection and Data Wrangling
- Video - How to Gather and Import Data
- Video - Data Wrangling
- Video - Tools for Data Wrangling
- Lab - Hands-On Lab: Load data into the Datasette from a CSV file
- Lab - Hands-on Lab: Load data into the Db2 Database from a CSV file
- Read - Summary and Highlights
- Quiz - Practice Quiz
- Quiz - Graded Quiz


#### ✔️ L3 - Querying Data, Performance Tuning, and Troubleshooting
- Video - Querying and Analyzing Data
- Video - Performance Tuning and Troubleshooting
- Lab - Lab: Explore your dataset using SQL queries using Datasette
- Lab - Hands-on Lab: Explore Your Dataset Using SQL Queries in DB2
- Read - Summary and Highlights
- Quiz - Practice Quiz
- Quiz - Graded Quiz


#### ✔️ L4 - Governance and Compliance
- Video - Governance and Compliance
- Read - Summary and Highlights
- Quiz - Practice Quiz
- Quiz - Graded Quiz
- Read - Overview of the DataOps Methodology


### ✅️ M4 - Career Opportunities and Data Engineering in Action
#### ✔️ L1 - Career Opportunities and Learning Paths
- Video - Career Opportunities in Data Engineering
- Read - Reading: Data Warehousing Specialist
- Read - Reading: Data Manager
- Video - Viewpoints: Get into Data Engineering
- Video - Data Engineering Learning Path
- Video - Viewpoints: What Do Employers Look for in a Data Engineer
- Video - Viewpoints: The Many Paths to Data Engineering
- Video - Viewpoints: Advice to Aspiring Data Engineers


#### ✔️ L2 - Module Quiz
- Read - Summary and Highlights
- Quiz - Practice Quiz
- Quiz - Graded Quiz


### ✅️ M5 - Final Project and Quiz
#### ✔️ L2 - Final Project
- Project - Final Project Submission Guidelines and Deliverables
- Review - Option 1: AI-Graded - Final Submission and Evaluation
- Review - Option 2: Peer-graded Assignment - Final Submission and Evaluation
- Review - Option 2: Peer-graded Assignment - Final Submission and Evaluation


#### ✔️ L3 - Final Quiz
- Quiz - Final Quiz
- Read - Congratulations and Next Steps

---

## M1C1 - Get started



### 01 - Welcome to the Google Data Analytics Certificate

XXX

### 02 - Reading: Course 1 Overview: Set Your Expectations

####  Program overview

1. Foundations: Data, Data, Everywhere (this course)
2. Ask Questions to Make Data-Driven Decisions
3. Prepare Data for Exploration
4. Process Data from Dirty to Clean
5. Analyze Data to Answer Questions
6. Share Data Through the Art of Visualization
7. Data Analysis with R Programming
8. Google Data Analytics Capstone: Complete a Case Study
9. Accelerate Your Job Search with AI
 
#### Course 1 content

Each course is broken into modules. Here’s a quick overview of the skills you'll gain in each of the four Course 1 modules. 

- Module 1: Introducing data analytics and analytical thinking

Data helps us make decisions in both everyday life and in business. In this part of the course, you’ll learn how data analysts use a variety of tools and skills to inform those decisions. You’ll also get to know more about this course and the overall program expectations.

- Module 2: The wonderful world of data

In this part of the course, you'll learn about the data life cycle and data analysis process. They are both relevant to your work in this program and on the job. You’ll also be introduced to applications that help guide data through the data analysis process.

- Module 3: Set up your data analytics toolbox

Spreadsheets, query languages, and data visualization tools are all a big part of a data analyst’s job. In this part of the course, you’ll learn the basic concepts to use them for data analysis. You’ll also understand how they work through interesting examples.

- Module 4: Become a fair and impactful data professional

In this part of the course, you’ll examine different types of businesses and the jobs and tasks that analysts do for them. You’ll also learn how a Google Data Analytics Certificate will help you meet many of the requirements for an analyst position with these organizations.

### 03 - Introduction to the Course

XXX

### 04 - Get Started with Your Google Data Analytics Certificate

XXX

### 05 - Reading: Evaluate Your Current Data Analytics Skills

#### Data analytics knowledge and skills 

Data analysts must have a comprehensive understanding of the data analytics process, as well as the technical skills that allow them to complete the data analysis process. In this section, you’ll consider questions about the data analytics process and specific technical skills to determine your readiness for the advanced certificate programs.

First, evaluate your knowledge of the data analytics process by considering whether the following statements apply to you:

- I have a thorough understanding of data-driven decision-making and how it helps organizations guide their business strategy based on facts. 
- I’m able to ask questions and make hypotheses about business problems and use them to guide me through the data analysis process.
- I know the steps to verify data credibility and perform data validation. 
- I understand data modeling and know how organizations use it as a tool to understand their data. 
- I can select and design visualizations that help me effectively communicate analysis insights to stakeholders. 

If the previous statements apply to you, you probably know the basics of the data analysis process. Continue reading to evaluate your technical skills.

Data analysts use a variety of tools, including software and programming languages, to analyze data. You will be most successful in an advanced certificate program if you’re able to use spreadsheets, SQL, Tableau, and R, which are covered in this program. Consider whether the following statements apply to you:

- I’m able to join data from multiple sources to use for data analysis.
- I can sort data in both a spreadsheet and a database.
- I’m able to clean data by ensuring it contains no duplicate or incorrect entries and is in the correct format.
- I know how to create data visualizations using a spreadsheet, Tableau, and R. 
- I can write a SQL command that would select several columns from a table.
- I understand packages in R and can select and install the packages I need to complete specific tasks.
