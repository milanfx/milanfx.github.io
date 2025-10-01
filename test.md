---
layout: page
title: Milanfx Study Notes
permalink: /xxx/
---




# Excel Filtering and Sorting Data

**Estimated Time Needed: 30 Minutes**

### Overview

In this lab, first you will learn how to use the Filter and Sort tools in Excel to filter and sort our data to enable us to control what information is displayed, and how it is displayed in our worksheets. Next, you will learn how to use some of the most common functions a Data Analyst might use; namely IF, IFS, COUNTIF, and SUMIF. Finally, you will learn how to use the VLOOKUP and HLOOKUP functions in Excel to reference data contained in both vertical and horizontal lookup tables. 

### Software

The instruction videos in this course use the full Excel Desktop version as this has all the available product features, but for the hands-on labs we will be using the free 'Excel for the web' version as this is available to everyone.

Although you can use the Excel Desktop software if you have access to this version, it is recommended that you use Excel for the web for the hands-on labs as the lab instructions specifically refer to this version, and there are some small differences in the interface and available features.

### Dataset

The first dataset used in this lab comes from the following source: https://dataplatform.cloud.ibm.com/exchange/public/entry/view/f8ccaf607372882403a37d9019b3abf4. This dataset is published by **IBM**, and includes fictitious customer demographics and sales data. 

The second dataset used in this lab comes from the following source: https://www.kaggle.com/sudalairajkumar/indian-startup-funding under a **[CC0: Public Domain license](https://creativecommons.org/publicdomain/zero/1.0/)**. 
Acknowledgement and thanks also goes to https://trak.in who were generous enough to share the data publicly for free.

We are using modified subsets of these datasets for the lab, so to follow the lab instructions successfully please use the datasets provided with the lab, rather than the datasets from their original sources.

The third dataset used in this lab is an internal dataset.

### Objectives

After completing this lab, you will be able to:

- Use the Filter and Sort tools
- Use IF, IFS, COUNTIF, and SUMIF functions for data analysis
- Use the VLOOKUP and HLOOKUP reference functions

## Exercise 1: Filtering and Sorting Data

In this exercise, you will learn how to use the Filter and Sort tools in Excel to filter and sort our data to enable us to control what information is displayed, and how it is displayed in our worksheets.

### Task A: Filtering data

To use Auto Filters to filter data:

**Step 1:** Download the file **[Customer_demographics_and_sales_Lab6.xlsx](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%206%20-%20Filtering%20and%20Sorting%20Data%20using%20Functions%20for%20Data%20Analysis/Customer_demographics_and_sales_Lab6.xlsx)**. Upload and open it using Excel for the web.

**Step 2:** Select **any cell** in the data, and click the **Data** tab, then click **Filter**.

**Step 3:** Click the **filter drop-down** in column **AG (Purchase_Status)**, and select **Filter...**.

**Step 4:** In the list, only select **Frequent** and click **OK**.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%206%20-%20Filtering%20and%20Sorting%20Data%20using%20Functions%20for%20Data%20Analysis/images/1.A.4.png" style="width:890px; max-height:500px; object-fit:contain;"></div></div>

**Step 5:** Click the **filter drop-down** in the column **AG**, and click **Clear Filter From “Purchase_Status”**.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%206%20-%20Filtering%20and%20Sorting%20Data%20using%20Functions%20for%20Data%20Analysis/images/1.A.5.png" style="width:890px; max-height:500px; object-fit:contain;"></div></div>

**Step 6:** Click the **filter drop-down** in column **AE (T_Type)**, and select **Filter...**.

**Step 7:** In the list, only select **Cancelled** and click **OK**.

**Step 8:** Click the **filter drop-down** in column **AF (Purchase_Touchpoint)**, and select **Filter...**.

**Step 9:** In the list, only select **Desktop** and click **OK**.

**Step 10:** On the **Data** tab, click **Clear**.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%206%20-%20Filtering%20and%20Sorting%20Data%20using%20Functions%20for%20Data%20Analysis/images/1.A.10.png" style="width:890px; max-height:500px; object-fit:contain;"></div></div>

To use Custom Filters to filter data:

- a. Click the **filter drop-down** in column **AD (Order_Value)**, then **Number Filters>Top 10...**.

- b. Change the value from **10 to 50** and Click **OK**.

- c. Click the **filter drop-down** in the column **AD**, and click **Clear Filter From “Order_Value”**.

### Task B: Sorting data

**Step 1:** On the **Data** tab, click Custom Sort to open a dialog box like below.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%206%20-%20Filtering%20and%20Sorting%20Data%20using%20Functions%20for%20Data%20Analysis/images/2.B.1.png" style="width:890px; max-height:500px; object-fit:contain;"></div></div>

**Step 2:** Click the **Column drop-down** of row **Sort By**, select **Order_Ship_Date**.

**Step 3:** Click the **Order drop-down** of row **Sort By**, select **Sort Ascending**.

**Step 4:** Click **Add**.

**Step 5:** Click the **Column drop-down** of row **Then By**, select **Order_Value**.

**Step 6:** Click the **Order drop-down** of row **Then By**, select **Sort Descending**.

**Step 7:** Click **OK**.

## Exercise 2: Useful Functions for Data Analysis

In this exercise, you will learn how to use some of the most common functions a Data Analyst might use; namely IF, IFS, COUNTIF, and SUMIF.

### Task A: Use of IF to apply one condition

**Step 1:** Select column **AF**, right-click, **Insert**.

**Step 2:** In cell **AF1**, type **Complete?**.

**Step 3:** In cell **AF2**, type **=IF(AE2="Complete","Yes","No")** and press Enter.

**Step 4:** Double-click the **Fill Handle of AF2** to copy down the column.

### Task B: Use of Nested IF to apply multiple conditions

**Step 1:** Select column **AE**, right-click, **Insert**.

**Step 2:** In cell **AE1**, type **Order Size (IF)**.

**Step 3:** In cell **AE2**, type **=IF(AD2>300,"Large",IF(AD2>100,"Medium",IF(AD2>0,"Small")))** and press **Enter**.

**Step 4:** Double-click the **Fill Handle of AE2** to copy down the column.

### Task C: Use of IFS to apply multiple conditions (alternative of Nested IF)

**Step 1:** Select column **AE**, right-click, **Insert**.

**Step 2:** In cell **AE1**, type **Order Size (IFS)**.

**Step 3:** In cell **AE2**, type **=IFS(AD2>300,"Large",AD2>100,"Medium",AD2>0,"Small")** and press **Enter**.

**Step 4:** Double-click the **Fill Handle of AE2** to copy down the column.

### Task D: Use of COUNTIF to count the number of cells that meet a specified criterion

**Step 1:** Select cell **BX2** and type **count VISA card**.

**Step 2:** Select cell **BY2** and type **=COUNTIF(N2:N195,"VISA")** and press **Enter**.

### Task E: Use of SUMIF function to sum the values within a specified range that meet a specified criterion

**Step 1:** Select cell **BX3** and type **sum Large order**.

**Step 2:** Select cell **BY3** and type **=SUMIF(AE2:AE195,"Large", AD2:AD195)** and press **Enter**.

- Formula: **=SUMIF(range, criteria, [sum range])**.

### Task F: Use of SUMIFS function to sum the values within a specified range that meet multiple specified criteria

**Step 1:** Select cell **BX4** and type **sum Large order with Baby Gen**.

**Step 2:** Select cell **BY4** and type **=SUMIFS(AD2:AD195, AE2:AE195,"Large", AL2:AL195,"BABY_BOOMERS")** and press **Enter**.

- Formula: **=SUMIFS ([sum range], range1, criteria1, range2, criteria2, ...)**.

## Exercise 3: Using the VLOOKUP and HLOOKUP Functions

In this exercise, you will learn how to use the VLOOKUP and HLOOKUP functions in Excel to reference data contained in both vertical and horizontal lookup tables. 

### Task A: Use of VLOOKUP to look up data in a table organized vertically

**Step 1:** Download the file **[indian_startup_funding_Lab6.xlsx](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%206%20-%20Filtering%20and%20Sorting%20Data%20using%20Functions%20for%20Data%20Analysis/indian_startup_funding_Lab6.xlsx)**. Upload and open it using Excel for the web.

**Step 2:** In cell **K2,L2,M2,** type **VLOOKUP, Startup Name, Amount in USD** respectively.

**Step 3:** Select and copy cells from **C9 to C15** and paste in cell **L3**.

**Step 4:** In cell **M3**, type **=VLOOKUP(L3, C2:I113, 7, FALSE)** and press **Enter**.

- Formula: **=VLOOKUP (value, table, col_index, [range_lookup])**.

**Step 5:** Hover over the bottom-right corner of cell **M3**, and drag the Fill Handle down to the cell **M9**.

**Step 6:** Select cells from **M3 to M9** and **select Number Format>Currency**.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%206%20-%20Filtering%20and%20Sorting%20Data%20using%20Functions%20for%20Data%20Analysis/images/3.A.png" style="width:890px; max-height:500px; object-fit:contain;"></div></div>

### Task B: Use of HLOOKUP to look up data in a table organized horizontally

**Step 1:** Download the file **[Personal_Monthly_Expenditure_Lab6.xlsx](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%206%20-%20Filtering%20and%20Sorting%20Data%20using%20Functions%20for%20Data%20Analysis/Personal_Monthly_Expenditure_Lab6.xlsx)**. Upload and open it using Excel for the web.

**Step 2:** In cell **J2,K2,L2,M2,** type **HLOOKUP, Month, Food & Dining, Health & Fitness** respectively.

**Step 3:** Select and copy cells from **A10 to A12** and paste in cell **K3**.

**Step 4:** In cell **L3**, type **=HLOOKUP(D1, A1:H14, 10, FALSE)** and press **Enter**.

- Formula: **=HLOOKUP (value, table, row_index, [range_lookup])**.

**Step 5:** Hover over the bottom-right corner of cell **L3**, and drag the Fill Handle down to the cell **L5**.

**Step 6:** Select cells from **L3 to L5** and **select Number Format>Currency**.

**Step 7:** In cell **M3**, type **=HLOOKUP(G1, A1:H14, 10, FALSE)** and press **Enter**.

**Step 8:** Hover over the bottom-right corner of cell **M3**, and drag the Fill Handle down to the cell **M5**.

**Step 9:** Select cells from **M3 to M5** and **select Number Format>Currency**.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%206%20-%20Filtering%20and%20Sorting%20Data%20using%20Functions%20for%20Data%20Analysis/images/3.B.png" style="width:890px; max-height:500px; object-fit:contain;"></div></div>

**Congratulations!**

You have completed this lab!



