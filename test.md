---
layout: page
permalink: /DS01M01/
---

### 🎯 Objectives

- **Topic01** - Use of **Sub-Queries** for Accessing **Multiple Tables**  
- **Topic02** - Application of **Implicit Joins** for Combining **Table Data**  
- **Topic03** - Implementation of **Table Aliases** for Simplifying **Query Syntax**  

### Topic01 - Use of Sub-Queries for Accessing Multiple Tables

- **Main Ideas:**
    - **Sub-Queries** allow retrieval of related data from **Multiple Tables** by nesting one query inside another.

- **Core Notes:**  
    - **Sub-Query Definition**:
        - A **Sub-Query** is a query within another query, used to retrieve data that will be used by the main (outer) query.
    - **Example 1** - Retrieving Employees by Department:
        - Query:  
            `SELECT * FROM Employees WHERE Department_ID IN (SELECT Department_ID FROM Departments);`
        - The **Outer Query** accesses the **Employees Table**.
        - The **Inner Query** accesses the **Departments Table** to filter results.
    - **Example 2** - Retrieving Employees by Location:
        - The **Employees Table** does not have location data.
        - The **Departments Table** includes **Location_ID**.
        - Query:  
            `SELECT * FROM Employees WHERE DEP_ID IN (SELECT DEP_ID_DEP FROM Departments WHERE LOC_ID='L0002');`
        - The sub-query filters departments based on **Location_ID**, and only employees in those departments are selected.
    - **Example 3** - Departments for Employees with High Salaries:
        - Objective: Retrieve **Department_ID** and **Department_Name** for employees earning more than **$70,000**.
        - Query:  
            `SELECT Department_ID, Department_Name FROM Departments WHERE Department_ID IN (SELECT Department_ID FROM Employees WHERE Salary > 70000);`
        - The **Inner Query** identifies departments of high-earning employees.
        - The **Outer Query** retrieves department details.

### Topic02 - Application of Implicit Joins for Combining Table Data

- **Main Ideas:**
    - **Implicit Joins** enable combining data from multiple tables using the **FROM Clause**, without explicitly using **JOIN Operators**.

- **Core Notes:**  
    - **Implicit Join Definition**:
        - Multiple tables are listed in the **FROM Clause**, and their relationship is defined in the **WHERE Clause**.
    - **Example 1** - Basic Implicit Join:
        - Query:  
            `SELECT * FROM Employees, Departments;`
        - Joins every row in **Employees** with every row in **Departments**.
        - This results in a **Full Join** producing a large number of rows.
    - **Limiting the Result Set**:
        - Use a **WHERE Clause** to filter matching rows.
        - Query:  
            `SELECT * FROM Employees, Departments WHERE Employees.DEP_ID = Departments.DEP_ID_DEP;`
        - This retrieves only rows where **Department_IDs** match between the two tables.
    - **Column Qualification**:
        - Prefix columns with table names to avoid ambiguity when both tables contain columns with identical names.
        - Example:  
            `Employees.DEP_ID` and `Departments.DEP_ID_DEP`
    - **Use Case**:
        - Implicit joins are efficient for combining related data but can become complex with more tables.

### Topic03 - Implementation of Table Aliases for Simplifying Query Syntax

- **Main Ideas:**
    - **Table Aliases** provide shorter names for tables, simplifying query writing and improving readability.

- **Core Notes:**  
    - **Alias Definition**:
        - Assigns a short name to a table, often a single letter, for convenience.
    - **Example 1** - Using Aliases in Joins:
        - Query:  
            `SELECT * FROM Employees E, Departments D WHERE E.DEP_ID = D.DEP_ID_DEP;`
        - **E** is an alias for **Employees**, and **D** is an alias for **Departments**.
        - The **WHERE Clause** uses these aliases to match department IDs.
    - **Example 2** - Selecting Specific Columns with Aliases:
        - Query:  
            `SELECT E.EMP_ID, D.DEP_NAME FROM Employees E, Departments D WHERE E.DEP_ID = D.DEP_ID_DEP;`
        - Prefixing column names with table aliases clarifies which table each column belongs to.
    - **Advantages**:
        - Simplifies long table names.
        - Increases readability.
        - Prevents column name conflicts when working with multiple tables.

### 📌 Takeaways

- **Sub-Queries** enable hierarchical data retrieval by embedding one query inside another.  
- **Implicit Joins** combine multiple tables using the **FROM Clause** and conditional logic in the **WHERE Clause**.  
- **Column Qualification** ensures clarity when tables share column names.  
- **Table Aliases** make SQL queries cleaner, more readable, and easier to maintain.  
- **Query Optimization** often involves balancing readability with efficiency, especially when using multiple tables.  
- **Practical SQL Queries** frequently combine **Sub-Queries** and **Implicit Joins** for flexible multi-table data access.  




