---
layout: page
permalink: /DS06M5/
---

## M5 - SQL and Python
- **01 - How to Access Databases using Python?**
- **02 - Writing Code using DB-API**
- **03 - Accessing Databases with SQL Magic**
- **04 - Analyzing Data with Python**
- **05 - Working with Real World Datasets**
- **06 - Getting Table and Column Details**

## 01 - How to Access Databases using Python?

### 🎯 Objectives
- **Topic01** - Accessing **Databases** with **Python**
- **Topic02** - Understanding **Python Database APIs** and **SQL APIs**
- **Topic03** - Exploring **Proprietary APIs** for SQL-Based **DBMS Systems**
- **Topic04** - Utilizing **Jupyter Notebooks** for **Data Analysis** and **Database Interaction**

### Topic01 - Accessing Databases with Python
- **Main Ideas:**
    - **Python** enables efficient **Database Access** for **Data Scientists** through a variety of **Tools**, **Libraries**, and **APIs**.

- **Core Notes:**
    - **Databases** are powerful tools for **Data Analysis** and **Storage** in **Data Science**.
    - **Python** can connect to databases to **Create Tables**, **Load Data**, **Query Data** using **SQL**, and **Analyze Results**.
    - **Cloud Instances** can be used to connect **Python Applications** to databases for remote **Data Access**.
    - **Python** offers a rich ecosystem with packages such as:
        - **NumPy** for **Numerical Computation**.
        - **Pandas** for **Data Manipulation**.
        - **matplotlib** for **Data Visualization**.
        - **SciPy** for **Scientific Computing**.
    - **Python** is **Open Source**, **Cross-Platform**, and **Easy to Learn** with a **Simple Syntax**.
    - **Platform Portability** allows Python programs to run across different systems without modification.

### Topic02 - Understanding Python Database APIs and SQL APIs
- **Main Ideas:**
    - **SQL APIs** and **Python DB APIs** define the interface between a **Python Application** and a **Database Management System (DBMS)**.

- **Core Notes:**
    - **API (Application Programming Interface)** is a set of **Functions** that enables a program to interact with a **Service**.
    - **SQL API** provides **Library Functions** to execute SQL statements and retrieve results from a **DBMS**.
    - **DB API** is a **Python Standard Interface** for **Database Connectivity**.
    - **API Calls** are used to:
        - Connect a program to a **DBMS**.
        - Send **SQL Statements** built as **Text Strings**.
        - Retrieve **Query Results** and **Status Information**.
        - Handle **Errors**.
        - Disconnect from the **Database**.
    - Example: A Python script sends a **SELECT** query through the **DB API**, retrieves the result set, checks the status, and then closes the connection.

### Topic03 - Exploring Proprietary APIs for SQL-Based DBMS Systems
- **Main Ideas:**
    - Various **DBMS Systems** use distinct **Proprietary APIs** for **Database Access** and **Integration**.

- **Core Notes:**
    - Each **Database System** provides its own **Library** or **API**.
    - Examples of **Proprietary APIs** include:
        - **MySQL C API** - Enables **Low-Level Access** to the **MySQL Client-Server Protocol** for **C Programs**.
        - **psycopg2 API** - Connects **Python Applications** to **PostgreSQL Databases**.
        - **IBM_DB API** - Interfaces **Python Applications** with **IBM DB2 Databases**.
        - **dblib API** - Connects to **Microsoft SQL Server Databases**.
        - **ODBC (Open Database Connectivity)** - Standard interface for **Windows-Based Database Access**.
        - **OCI (Oracle Call Interface)** - Used by **Oracle Databases**.
        - **JDBC (Java Database Connectivity)** - Used by **Java Applications** for **Database Access**.

### Topic04 - Utilizing Jupyter Notebooks for Data Analysis and Database Interaction
- **Main Ideas:**
    - **Jupyter Notebooks** provide an **Interactive Environment** for **Programming**, **Visualization**, and **Database Operations**.

- **Core Notes:**
    - **Jupyter Notebook** is an **Open-Source Web Application** that supports live **Code**, **Equations**, **Visualizations**, and **Narrative Text**.
    - **Notebook Interfaces** include:
        - **Mathematica Notebook**
        - **Maple Worksheet**
        - **Matlab Notebook**
        - **IPython Jupyter**
        - **R Markdown**
        - **Apache Zeppelin**
        - **Apache Spark Notebook**
        - **Databricks Cloud**
    - **Advantages of Jupyter Notebooks**:
        - Support for over **40 Programming Languages**, including **Python**, **R**, **Julia**, and **Scala**.
        - Easy **Sharing** via **Email**, **Dropbox**, **GitHub**, or the **Jupyter Notebook Viewer**.
        - Production of **Rich Interactive Outputs** (HTML, Images, Videos, LaTeX).
        - Integration with **Big Data Tools** such as **Apache Spark**, **scikit-learn**, **pandas**, **ggplot2**, and **TensorFlow**.
    - Example: A data scientist uses **Python Code** in a **Jupyter Notebook** to connect to a **Database**, execute **SQL Queries**, and visualize results with **matplotlib**.

### 📌 Takeaways
- **Python** simplifies **Database Connectivity** through its **DB API** and rich **Ecosystem** of **Data Science Libraries**.  
- **SQL APIs** serve as intermediaries between **Applications** and **DBMS**, enabling **Query Execution** and **Result Retrieval**.  
- **Proprietary APIs** like **psycopg2**, **IBM_DB**, and **ODBC** provide system-specific **Database Access** capabilities.  
- **Jupyter Notebooks** enhance **Data Analysis** workflows by combining **Code Execution**, **Visualization**, and **Documentation** in one interface.  

## 02 - Writing Code using DB-API

### 🎯 Objectives
- **Topic01** - Fundamental Concepts of **Python DB-API** for Database Access  
- **Topic02** - Role of **Connection Objects** and **Cursor Objects** in Database Operations  
- **Topic03** - Steps for **Writing Python Code** to Query Databases Using DB-API  

### Topic01 - Fundamental Concepts of Python DB-API for Database Access
- **Main Ideas:**
    - **Python DB-API** standardizes **Database Connectivity**, enabling code portability across multiple **Relational Databases**.

- **Core Notes:**  
    - **DB-API** is the **Python Standard API** for accessing **Relational Databases**.  
    - It allows writing a single program that works with multiple database systems.  
    - Learning **DB-API Functions** enables users to apply the same logic across any database supported by Python.  
    - **Advantages of DB-API**:
        - **Easy Implementation** and **Comprehension**.  
        - **Consistency** among Python database modules.  
        - **Code Portability** across databases.  
        - **Broader Database Connectivity** from Python.  
    - Each **Database System** has its own **Library** for use with Python applications:
        - **IBM_DB** connects to **IBM DB2 Database**.  
        - **MySQL Connector Python** connects to **MySQL Database**.  
        - **psycopg2** connects to **PostgreSQL Database**.  
        - **PyMongo** connects to **MongoDB Database**.  

### Topic02 - Role of Connection Objects and Cursor Objects in Database Operations
- **Main Ideas:**
    - **Connection Objects** and **Cursor Objects** are central to managing **Database Transactions** and **Query Execution** in **Python DB-API**.

- **Core Notes:**  
    - **Connection Objects** are used to **Establish Connections** and **Manage Transactions** with databases.  
    - **Cursor Objects** are used to **Run Queries** and **Retrieve Results**.  
    - **DB-API Connect Constructor** creates a **Connection Object**, which is used by multiple **Connection Methods**:
        - **cursor()** - Returns a new **Cursor Object**.  
        - **commit()** - Commits any **Pending Transaction** to the database.  
        - **rollback()** - Reverts the database to the **Start of a Pending Transaction**.  
        - **close()** - Closes the **Database Connection**.  
    - **Cursors** are not isolated within the same connection:
        - Changes made by one cursor are **Immediately Visible** to other cursors under the same connection.  
        - **Isolation Behavior** across connections depends on **Transaction Implementation**.  
    - **Database Cursor** acts as a **Control Structure** for traversing database records:
        - Similar to a **File Handle** in programming.  
        - **Open Cursor** to access query results, and **Close Cursor** to end access.  
        - **Cursor Position** tracks progress through query results.  
    - Example:  
        - The program opens a **Cursor**, fetches data row by row, and then closes it to release resources.  

### Topic03 - Steps for Writing Python Code to Query Databases Using DB-API
- **Main Ideas:**
    - **Python DB-API Code** follows a structured process to connect, query, retrieve, and close database connections efficiently.

- **Core Notes:**  
    - **Python Application** uses **DB-API** to query databases within **Jupyter Notebooks**.  
    - **Steps to Write DB-API Code**:
        1. **Import Database Module** using the **connect() API**.  
        2. **Open Connection** using the **connect() Constructor** with parameters:
            - **Database Name**, **Username**, and **Password**.  
        3. **Create Cursor Object** from the **Connection Object**.  
        4. **Run Queries** using the **Cursor** and **Fetch Results**.  
        5. **Close Connection** after completing queries to release resources.  
    - **Closing Connections** is essential to prevent **Resource Leaks** from unused database connections.  
    - Example:  
        - The user imports **psycopg2**, connects to **PostgreSQL**, executes a **SELECT** query with a cursor, fetches data, and closes the connection.  

### 📌 Takeaways
- **DB-API** standardizes **Python Database Programming**, ensuring code reusability and cross-database compatibility.  
- **Connection Objects** manage **Database Sessions** and **Transactions**, while **Cursor Objects** handle **Query Execution** and **Result Retrieval**.  
- **Database Cursors** function like **File Handles**, providing controlled access to **Query Results**.  
- **Proper Connection Management** through opening, committing, and closing ensures **Efficient Resource Utilization** and **System Stability**.  

## 03 - Accessing Databases with SQL Magic
## 04 - Analyzing Data with Python
## 05 - Working with Real World Datasets
## 06 - Getting Table and Column Details
