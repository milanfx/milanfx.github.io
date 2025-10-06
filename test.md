---
layout: page
permalink: /DE01M01/
---

## Note-M1-Data-Science-Introduction

- 01 - Course Introduction
- 02 - Data Science Definition
- 03 - Data Science Fundamentals
- 04 - Data Science Paths
- 05 - Data Scientist Advice
- 06 - Data Science Summary

## 🧩 01 - Course Introduction

### 🎯 Objectives

1. Define what a **Data Repository** is and describe its purpose  
2. Distinguish between **Databases**, **Data Warehouses**, and **Big Data Stores**  
3. Compare **Relational (RDBMS)** and **Non-Relational (NoSQL)** databases  
4. Explain the **ETL Process** and its role in data integration  
5. Describe how **Data Repositories** support **Analytics** and **Business Intelligence**  

### 1. Define what a Data Repository is and describe its purpose

- **Main Ideas:**
 - A data repository is a structured environment for storing, managing, and retrieving data.
 - It serves as the foundation for reporting, analytics, and business operations.

- **Core Notes:**  
  - A **Data Repository** is a system that collects and organizes data for future use in **operations** or **analysis**.  
  - It can range from a **single database** to a **large-scale infrastructure** containing multiple databases.  
  - The main goal is to **isolate, organize, and maintain** data to ensure it is accessible and analyzable.  
  - Data repositories enhance the **efficiency**, **credibility**, and **accuracy** of data reporting and analytics.  
  - They also serve as **data archives** for long-term storage and compliance.  
    - xxxx
    - xxxx
    - xxxx

### 2. Distinguish between Databases, Data Warehouses, and Big Data Stores

- **Main Ideas:**
    - These three types of repositories differ in structure, purpose, and scale.
    - Each serves specific organizational needs, from daily transactions to large-scale analytics.

- **Core Notes:**  
    - **Databases:**  
        - Designed for **input, storage, search, retrieval, and modification** of data.  
        - Managed by a **Database Management System (DBMS)** that allows querying and updates.  
        - Example query: finding customers inactive for six months.  
        - Suitable for **operational data** and **transactional systems**.  
    - **Data Warehouses:**  
        - Serve as **central repositories** integrating data from multiple sources.  
        - Use the **ETL Process** (Extract, Transform, Load) to consolidate data into a single analytical database.  
        - Support **analytics** and **business intelligence (BI)** tasks.  
        - Traditionally built on **relational models**, though **non-relational** approaches are increasingly used.  
    - **Big Data Stores:**  
        - Designed for **massive, distributed data processing and storage**.  
        - Handle **high-volume**, **high-velocity**, and **high-variety** data.  
        - Commonly used in contexts involving **cloud computing**, **IoT**, and **social media** data streams.  

### 3. Compare Relational (RDBMS) and Non-Relational (NoSQL) databases

- **Main Ideas:**
    - Relational databases follow structured schemas; non-relational databases offer flexibility and scalability.
    - The choice depends on data type, structure, and performance needs.

- **Core Notes:**  
    - **Relational Databases (RDBMS):**  
        - Organize data into **tables (rows and columns)** with **defined schemas**.  
        - Use **Structured Query Language (SQL)** for data management.  
        - Optimized for **complex queries** and **transactions** involving multiple tables.  
        - Examples: **MySQL**, **PostgreSQL**, **Oracle Database**.  
    - **Non-Relational Databases (NoSQL):**  
        - “Not Only SQL” systems supporting **schema-less**, **flexible** data structures.  
        - Designed for **speed**, **scalability**, and **variety** of data types.  
        - Essential for handling **unstructured** or **semi-structured data** (e.g., JSON, key-value pairs).  
        - Examples: **MongoDB**, **Cassandra**, **Couchbase**, **HBase**.  
    - **Use Cases:**  
        - RDBMS → Best for **structured enterprise data** and **transactional systems**.  
        - NoSQL → Best for **Big Data**, **IoT**, and **cloud-based distributed systems**.  

### 4. Explain the ETL Process and its role in data integration

- **Main Ideas:**
    - The ETL process integrates data from multiple sources into a unified repository.
    - It ensures data consistency and readiness for analysis.

- **Core Notes:**  
    - **ETL (Extract, Transform, Load)** is a three-step process:  
        1. **Extract** – Gather data from multiple internal and external sources.  
        2. **Transform** – Clean, validate, and convert data into a standardized, usable format.  
        3. **Load** – Insert transformed data into the **Data Warehouse** or **Repository**.  
    - ETL improves **data quality** and ensures that datasets are **consistent**, **accurate**, and **analysis-ready**.  
    - Modern ETL processes often include **real-time streaming** and **cloud integration**.  
    - ETL forms the backbone of **business intelligence pipelines**, enabling unified data insights.  

### 5. Describe how Data Repositories support Analytics and Business Intelligence

- **Main Ideas:**
    - Data repositories enable efficient data analysis, visualization, and decision-making.
    - They form the core of enterprise data management strategies.

- **Core Notes:**  
    - Repositories isolate and structure data to make **reporting** and **analytics** easier and more credible.  
    - They support **querying**, **trend analysis**, **data mining**, and **machine learning** applications.  
    - **Data Warehouses** act as the analytical hub, enabling **organization-wide access** to unified data.  
    - **Big Data Stores** expand analytical capacity to include **real-time insights** and **massive data volumes**.  
    - Together, these systems empower organizations to make **data-driven decisions** and uncover new business opportunities.  

### 📌 Takeaways

1. A **Data Repository** is a centralized environment for storing, managing, and analyzing data.  
2. **Databases** manage daily operational data; **Data Warehouses** consolidate data for analytics; **Big Data Stores** handle large-scale distributed data.  
3. **RDBMS** systems use structured schemas and SQL, while **NoSQL** systems offer flexibility for modern data needs.  
4. The **ETL Process**—Extract, Transform, Load—is essential for integrating diverse data sources into a unified analytical platform.  
5. Data repositories are fundamental to **Business Intelligence (BI)**, ensuring reliable reporting and decision-making.  
6. The evolution of repositories reflects the shift toward **Big Data**, **Cloud Computing**, and **Scalable Analytics**.  
7. Effective data management depends on choosing the right repository type for the organization’s data structure and goals.  


## 🧩 02 - Data Science Definition

### 🎯 Objectives
1. Define what a **Data Repository** is and describe its purpose  
2. Distinguish between **Databases**, **Data Warehouses**, and **Big Data Stores**  
3. Compare **Relational (RDBMS)** and **Non-Relational (NoSQL)** databases  
4. Explain the **ETL Process** and its role in data integration  
5. Describe how **Data Repositories** support **Analytics** and **Business Intelligence**  

### 1. Define what a Data Repository is and describe its purpose
- **Main Ideas:**
    - A data repository is a structured environment for storing, managing, and retrieving data.
    - It serves as the foundation for reporting, analytics, and business operations.

- **Core Notes:**  
    - A **Data Repository** is a system that collects and organizes data for future use in **operations** or **analysis**.  
    - It can range from a **single database** to a **large-scale infrastructure** containing multiple databases.  
    - The main goal is to **isolate, organize, and maintain** data to ensure it is accessible and analyzable.  
    - Data repositories enhance the **efficiency**, **credibility**, and **accuracy** of data reporting and analytics.  
    - They also serve as **data archives** for long-term storage and compliance.  

### 2. Distinguish between Databases, Data Warehouses, and Big Data Stores
- **Main Ideas:**
    - These three types of repositories differ in structure, purpose, and scale.
    - Each serves specific organizational needs, from daily transactions to large-scale analytics.

- **Core Notes:**  
    - **Databases:**  
        - Designed for **input, storage, search, retrieval, and modification** of data.  
        - Managed by a **Database Management System (DBMS)** that allows querying and updates.  
        - Example query: finding customers inactive for six months.  
        - Suitable for **operational data** and **transactional systems**.  
    - **Data Warehouses:**  
        - Serve as **central repositories** integrating data from multiple sources.  
        - Use the **ETL Process** (Extract, Transform, Load) to consolidate data into a single analytical database.  
        - Support **analytics** and **business intelligence (BI)** tasks.  
        - Traditionally built on **relational models**, though **non-relational** approaches are increasingly used.  
    - **Big Data Stores:**  
        - Designed for **massive, distributed data processing and storage**.  
        - Handle **high-volume**, **high-velocity**, and **high-variety** data.  
        - Commonly used in contexts involving **cloud computing**, **IoT**, and **social media** data streams.  

### 3. Compare Relational (RDBMS) and Non-Relational (NoSQL) databases
- **Main Ideas:**
    - Relational databases follow structured schemas; non-relational databases offer flexibility and scalability.
    - The choice depends on data type, structure, and performance needs.

- **Core Notes:**  
    - **Relational Databases (RDBMS):**  
        - Organize data into **tables (rows and columns)** with **defined schemas**.  
        - Use **Structured Query Language (SQL)** for data management.  
        - Optimized for **complex queries** and **transactions** involving multiple tables.  
        - Examples: **MySQL**, **PostgreSQL**, **Oracle Database**.  
    - **Non-Relational Databases (NoSQL):**  
        - “Not Only SQL” systems supporting **schema-less**, **flexible** data structures.  
        - Designed for **speed**, **scalability**, and **variety** of data types.  
        - Essential for handling **unstructured** or **semi-structured data** (e.g., JSON, key-value pairs).  
        - Examples: **MongoDB**, **Cassandra**, **Couchbase**, **HBase**.  
    - **Use Cases:**  
        - RDBMS → Best for **structured enterprise data** and **transactional systems**.  
        - NoSQL → Best for **Big Data**, **IoT**, and **cloud-based distributed systems**.  

### 4. Explain the ETL Process and its role in data integration
- **Main Ideas:**
    - The ETL process integrates data from multiple sources into a unified repository.
    - It ensures data consistency and readiness for analysis.

- **Core Notes:**  
    - **ETL (Extract, Transform, Load)** is a three-step process:  
        1. **Extract** – Gather data from multiple internal and external sources.  
        2. **Transform** – Clean, validate, and convert data into a standardized, usable format.  
        3. **Load** – Insert transformed data into the **Data Warehouse** or **Repository**.  
    - ETL improves **data quality** and ensures that datasets are **consistent**, **accurate**, and **analysis-ready**.  
    - Modern ETL processes often include **real-time streaming** and **cloud integration**.  
    - ETL forms the backbone of **business intelligence pipelines**, enabling unified data insights.  

### 5. Describe how Data Repositories support Analytics and Business Intelligence
- **Main Ideas:**
    - Data repositories enable efficient data analysis, visualization, and decision-making.
    - They form the core of enterprise data management strategies.

- **Core Notes:**  
    - Repositories isolate and structure data to make **reporting** and **analytics** easier and more credible.  
    - They support **querying**, **trend analysis**, **data mining**, and **machine learning** applications.  
    - **Data Warehouses** act as the analytical hub, enabling **organization-wide access** to unified data.  
    - **Big Data Stores** expand analytical capacity to include **real-time insights** and **massive data volumes**.  
    - Together, these systems empower organizations to make **data-driven decisions** and uncover new business opportunities.  

### 📌 Takeaways
1. A **Data Repository** is a centralized environment for storing, managing, and analyzing data.  
2. **Databases** manage daily operational data; **Data Warehouses** consolidate data for analytics; **Big Data Stores** handle large-scale distributed data.  
3. **RDBMS** systems use structured schemas and SQL, while **NoSQL** systems offer flexibility for modern data needs.  
4. The **ETL Process**—Extract, Transform, Load—is essential for integrating diverse data sources into a unified analytical platform.  
5. Data repositories are fundamental to **Business Intelligence (BI)**, ensuring reliable reporting and decision-making.  
6. The evolution of repositories reflects the shift toward **Big Data**, **Cloud Computing**, and **Scalable Analytics**.  
7. Effective data management depends on choosing the right repository type for the organization’s data structure and goals.  
