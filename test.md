---
layout: page
title: Milanfx Study Notes
permalink: /xxx/
---



# Excel Spreadsheet Basics

**Estimated Time Needed: 20 Minutes**

### Overview

To get started with a spreadsheet app, you need to know:

- Some of the common terminology around it
- What its key features are
- How to use some basic tools on the ribbon
- How to move around a worksheet
- How to select data in it. 

In this lab, you will go through some basic spreadsheet elements, explore the ribbon, navigate around a worksheet and select data.

### Software Used in this Lab

The instruction videos in this course use the full Excel Desktop version as this has all the available product features, but for the hands-on labs we will be using the free 'Excel for the web' version as this is available to everyone.

Although you can use the Excel Desktop software if you have access to this version, <ins>it is recommended that you use Excel for the web for the hands-on labs</ins> as the lab instructions specifically refer to this version, and there are some small differences in the interface and available features.

### Dataset Used in this Lab

The dataset used in this lab comes from the following source: https://www.kaggle.com/sudalairajkumar/indian-startup-funding under a **[CC0: Public Domain license](https://creativecommons.org/publicdomain/zero/1.0/)**. 
Acknowledgement and thanks also goes to https://trak.in who were generous enough to share the data publicly for free.

We are using a modified subset of that dataset for the lab, so to follow the lab instructions successfully please use the dataset provided with the lab, rather than the dataset from the original source.

### Objectives

After completing this lab, you will be able to:

- Understand and use the basic elements of a spreadsheet.
- Explore the ribbon, navigate around a worksheet and select data.

## Exercise 1: Introduction to Basic Spreadsheet Elements

In this exercise, you will learn about some common spreadsheet elements.

**Step 1:** Open **Excel for the web** (https://excel.cloud.microsoft/). Click on **Create blank workbook**.

<div style="display: inline-grid; border: 3px solid Purple; margin-bottom:20px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IUozSPx1qIfrFUfHow33_g/Lab2-Spreadsheet%20Basics-NewBlankWorksheet.png" style="max-height:600px; min-height:300px; max-width:900px; min-width:450px; width:auto; height:auto; object-fit:contain;">
</div>

**Step 2:** The new blank workbook will automatically be saved in Excel for the web as **Book 1**. To rename the workbook to something more meaningful, click **File**, **Save As**, then choose **Rename**.

<div style="display: inline-grid; border: 3px solid Purple; margin-bottom:20px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%202%20-%20Spreadsheet%20basics/images/1.2.jpg" style="max-height:600px; min-height:300px; max-width:900px; min-width:450px; width:auto; height:auto; object-fit:contain;">
</div>

**Step 3:** In the file name box, type **Personal_Monthly_Expenditure_Lab2** and click **OK**.

<div style="display: inline-grid; border: 3px solid Purple; margin-bottom:20px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%202%20-%20Spreadsheet%20basics/images/1.3.png" style="max-height:600px; min-height:300px; max-width:900px; min-width:450px; width:auto; height:auto; object-fit:contain;">
</div>

**Step 4:** In the saved workbook, you will have one worksheet opened, named *Sheet1*. Click **+** once to add another worksheet. Then, double-click the sheet name tab for **Sheet1** and rename it to **Expense - 2019**. Similarly, rename **Sheet2** as **Expense - 2018**.

<div style="display: inline-grid; border: 3px solid Purple; margin-bottom:20px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%202%20-%20Spreadsheet%20basics/images/1.4.png" style="max-height:600px; min-height:300px; max-width:900px; min-width:450px; width:auto; height:auto; object-fit:contain;">
</div>

**Step 5:** To maintain an appropriate worksheet tab sequence, click on the worksheet tab **Expense - 2018**, then drag and drop it before the **Expense - 2019** tab.

<div style="display: inline-grid; border: 3px solid Purple; margin-bottom:20px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%202%20-%20Spreadsheet%20basics/images/1.5.gif" style="max-height:600px; min-height:300px; max-width:900px; min-width:450px; width:auto; height:auto; object-fit:contain;">
</div>

**Step 6:** Click on the **Expense - 2018** tab. Select an entire column by clicking on **B** in the top of the worksheet, then select an entire row by clicking on the number **5** in the left of the worksheet. Click cell **B5**, and a green outline will appear around the cell. Now check if you have clicked the correct cell by looking at the cell name box in the top left corner, circled in red below.

<div style="display: inline-grid; border: 3px solid Purple; margin-bottom:20px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%202%20-%20Spreadsheet%20basics/images/1.6.png" style="max-height:600px; min-height:300px; max-width:900px; min-width:450px; width:auto; height:auto; object-fit:contain;">
</div>

**Step 7:** Select several cells in the same row, such as A1:D1 by clicking cell **A1** and then drag the cursor across to **D1**. Similarly, select a cell range in the same column, such as A1:A5 by clicking **A1** and dragging the cursor down to **A5**.

<div style="display: inline-grid; border: 3px solid Purple; margin-bottom:20px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%202%20-%20Spreadsheet%20basics/images/1.7.gif" style="max-height:600px; min-height:300px; max-width:900px; min-width:450px; width:auto; height:auto; object-fit:contain;">
</div>

**Step 8:** Now select a cell range which includes several rows and columns together, such as A1:C5 by clicking **A1** and then dragging the cursor across and down to cell **C5**.

<div style="display: inline-grid; border: 3px solid Purple; margin-bottom:20px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%202%20-%20Spreadsheet%20basics/images/1.8.gif" style="max-height:600px; min-height:300px; max-width:900px; min-width:450px; width:auto; height:auto; object-fit:contain;">
</div>

## Exercise 2:  Explore the Ribbon, Navigate around a Worksheet, and Select Data

In this exercise, you will explore the ribbon, then navigate around a worksheet, and select data.

### Task A: Explore the ribbon

**Step 1:** Download the file **[indian_startup_funding_Lab2.xlsx](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%202%20-%20Spreadsheet%20basics/indian_startup_funding_Lab2.xlsx)**.

**Step 2:** To open a sample file in Excel for the web, click the **App Launcher** (cube of dots) in the top left corner. Click **Excel**, and then click **Upload and open...** and select the **indian_startup_funding_Lab2.xlsx** file.

<div style="display: inline-grid; border: 3px solid Purple; margin-bottom:20px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%202%20-%20Spreadsheet%20basics/images/2A.1.png" style="max-height:600px; min-height:300px; max-width:900px; min-width:450px; width:auto; height:auto; object-fit:contain;">
</div>

**Step 3:** Click each of the following tabs in the ribbon; **File, Home, Insert, Formulas, Data, Review, View** to explore each of them and get acquainted with the ribbon. Double-click any of the tabs to hide the ribbon, then do the same again to unhide it.

### Task B: Navigate around a worksheet

**Step 1:** Click on **any cell** and move around the worksheet using the arrow keys; **Up, Down, Left, Right**.

<div style="display: inline-grid; border: 3px solid Purple; margin-bottom:20px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%202%20-%20Spreadsheet%20basics/images/2B.1.gif" style="max-height:600px; min-height:300px; max-width:900px; min-width:450px; width:auto; height:auto; object-fit:contain;">
</div>

**Step 2:** Click **Page Down** twice, and then **Page Up** twice to move around a bit faster, which is useful if you have lots of rows of data.

**Step 3:** Click and drag the **horizontal scroll bar** and then the **vertical scroll bar** to move even quicker up, down, and across a large datasheet.

**Step 4:** Try out these useful shortcuts in your worksheet:

- Press **CTRL+End** to take you to the cell at the end of your data in the worksheet.
- Press **CTRL+Home** to take you back to the start of the data in the worksheet (i.e. cell A2).
- Press **CTRL+Down Arrow** to take you to the end of the column you’re in
- Press **CTRL+Up Arrow** to take you back to the top of the column.

### Task C: Select data

Perform the following steps to learn how to select different parts of your data (you can use the mouse to select cells if you prefer):

**Step 1:** <ins>To select cells in a single row:</ins> Select cell **A1**, then select cells **A1 to D1** by using **SHIFT+right arrow**.

- <ins>To select cells in a single column:</ins> Select cell **A1**, then select cells **A1 to A10** by using **SHIFT+down arrow**.

<div style="display: inline-grid; border: 3px solid Purple; margin-bottom:20px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%202%20-%20Spreadsheet%20basics/images/2C.1.gif" style="max-height:600px; min-height:300px; max-width:900px; min-width:450px; width:auto; height:auto; object-fit:contain;">
</div>

**Step 2:** <ins>To select multiple contiguous cols/rows:</ins>  Select column **A**, and use **SHIFT+ right arrow** to reach column **E**.

**Step 3:** <ins>To select multiple non-contiguous cols/rows:</ins> Select column **A**, then hold **CTRL** and select column **E**.

**Step 4:** <ins>To select the entire worksheet:</ins> Click the **corner button** (small grey triangle in top left corner of the worksheet).

- <ins>To select all your data:</ins> Select any cell in the data, then press **CTRL+A**.

**NOTE:** The first time you press CTRL+A, it selects the current region if the worksheet contains data, the second time it selects the current data region and its header row, and the third time it selects the entire worksheet.

<div style="display: inline-grid; border: 3px solid Purple; margin-bottom:20px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%202%20-%20Spreadsheet%20basics/images/2C.4.gif" style="max-height:600px; min-height:300px; max-width:900px; min-width:450px; width:auto; height:auto; object-fit:contain;">
</div>

**Congratulations!**

You have completed Lab 2, and you are ready for the next topic.





