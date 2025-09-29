---
layout: page
title: Milanfx Study Notes
permalink: /xxx/
---


# Excel Entering and Formatting Data

**Estimated Time Needed: 30 Minutes**

### Overview

In this lab, first you will learn some of the viewing options in Excel, and then learn how to enter and edit data in cells. Then, you will learn how to move, copy, paste, and fill data, and how to format cells and cell data in a worksheet.

### Software Used in this Lab

The instruction videos in this course use the full Excel Desktop version as this has all the available product features, but for the hands-on labs we will be using the free 'Excel for the web' version as this is available to everyone.

Although you can use the Excel Desktop software if you have access to this version, <ins>it is recommended that you use Excel for the web for the hands-on labs</ins> as the lab instructions specifically refer to this version, and there are some small differences in the interface and available features.

### Dataset Used in this Lab

The first dataset used in this lab comes from the following source: https://www.kaggle.com/sudalairajkumar/indian-startup-funding under a **[CC0: Public Domain license](https://creativecommons.org/publicdomain/zero/1.0/)**. Acknowledgement and thanks also goes to https://trak.in who were generous enough to share the data publicly for free.

We are using a modified subset of that dataset for the lab, so to follow the lab instructions successfully please use the dataset provided with the lab, rather than the dataset from the original source.

The second dataset used in this lab is an internal dataset.

### Objectives

After completing this lab, you will be able to:

- Use viewing options, and enter and edit data
- Copy and fill data, and format cells and data

## Exercise 1: Viewing, Entering and Editing Data

In this exercise, you will learn some of the viewing options in Excel, how to enter and edit data in cells.

### Task A: Viewing Data

**Step 1:** Download the file **[indian_startup_funding_Lab3.xlsx](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%203%20-%20Entering%20and%20Formatting%20Data/indian_startup_funding_Lab3.xlsx)**. Upload and open it using Excel for the web.

**Step 2:** Select **F20:H26** (if required, use the vertical and horizontal scroll bars to bring the selected cell range area to the center of the screen). Hold **CTRL and +** to zoom in closer to the specific area of the data. Then hold **CTRL and -** to zoom the worksheet back out to its original size. (**NOTE:** **Zoom to Selection** which is found under the **View** tab of Excel Desktop, is not available for Excel for the web)

**Step 3:** On the ribbon, click **View, Freeze Panes, Freeze Top Row**. Now you have headings in your columns like a header row, which will remain static on screen while you move down the worksheet. Next, click **Unfreeze Panes**, and click **Freeze First Column**. The *Sr No* column will remain static on the screen while you move right across the worksheet. Lastly, click **Unfreeze Panes** to end this step.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%203%20-%20Entering%20and%20Formatting%20Data/images/1A.3.png" width="400"></div>

**Step 4:** To freeze both the top row and the first column at the same time, select cell **B2** and click **View, Freeze Panes, Freeze Panes**.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%203%20-%20Entering%20and%20Formatting%20Data/images/1A.4.gif" width="800"></div>

**Step 5:** You can open multiple workbooks in multiple browser tabs in Excel for the web, and to switch between them, you just click each browser tab. (In Excel Desktop you have to click the **View** tab, then click **Switch Windows**)

### Task B: Entering Data

**Step 1:** Download the file **[Personal_Monthly_Expenditure_Lab3.xlsx](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%203%20-%20Entering%20and%20Formatting%20Data/Personal_Monthly_Expenditure_Lab3.xlsx)**(This is a blank worksheet where you are required to complete the tasks outlined below). Upload and open it using Excel for the web. Go to the **Expense - 2018** worksheet.

**Step 2:** In cell **A1**, type **Month** and press **Tab**. Then type **Housing** and press **Tab**, type **Food & Dining**, and press **Tab**, type **Personal**, and press **Tab**, type **Auto & Transport**, then press **Tab**, type **Health & Fitness**, then press **Tab**. You are now done with the header row.

**Step 3:** To enter some data as rows in column **A**, in **A2**, type **Jan** and press **Enter**. Then type **Feb**, and press **Enter**, type **Mar**, and press **Enter**, type **Apr**, and press **Enter**.

**Step 4:** To add another column between the **Housing** and **Food & Dining**, select column **C**, then right-click column **C**, and choose **Insert Columns**. In the top row header cell **C1**, type **Bills & Utilities**.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%203%20-%20Entering%20and%20Formatting%20Data/images/1B.4.png" width="800"></div>

**Step 5:** Select columns **A to G**, then double-click the divider between **A** and **B** to adjust the column widths.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%203%20-%20Entering%20and%20Formatting%20Data/images/1B.5.gif" width="800"></div>

### Task C: Editing Data

**Step 1:** Select cell **C1** and press **Backspace** to clear the contents. Then type **Bills**. 

**Step 2:** Click **Undo** to undo the change.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%203%20-%20Entering%20and%20Formatting%20Data/images/1C.2.png" width="400"></div>

## Exercise 2: Copying, Filling, and Formatting Cells and Data

In this exercise, you will learn how to move, copy, paste, and fill data, and how to format cells and cell data in a worksheet.

### Task A: Copying and Filling Data

**Step 1:** Select **A2:A5**. Hover over the edge of the selected cells to get the **Move** pointer and then drag the selection to move the selected cells to **B6**. Click **Undo**.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%203%20-%20Entering%20and%20Formatting%20Data/images/2A.1.png" width="400"></div>

**Step 2:** Select cell **A5**. Hover over the bottom right corner of cell **A5** to get the **+ (Fill Handle)** symbol, then drag to **A13**.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%203%20-%20Entering%20and%20Formatting%20Data/images/2A.2.gif" width="400"></div>

**Step 3:** On the **Expense - 2018** sheet, select **A1:G13** and press **CTRL+C**. Then on the **Expense - 2019** sheet, select cell **A1** and press **CTRL+V**. 

**Step 4:** Select cell **A1** and press **CTRL+A** to select the whole datasheet. On the **Home** tab, in the **Cells** group, click the drop-down arrow under **Format**, and click **Auto-Fit Column Width**.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%203%20-%20Entering%20and%20Formatting%20Data/images/2A.4.png" width="800"></div>

### Task B: Formatting Cells and Data

Download the file **[Data_for_Personal_Monthly_Expenditure_Lab3.xlsx](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/wjEWjWZpHIiN7j5Ch8L00Q/Data-for-Personal-Monthly-Expenditure-Lab3.xlsx)**, which contains data for the Expense - 2019 sheet.

Copy the values from **B2:G13** and paste them into your existing Expense - 2019 sheet, which should then look like this:

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/xhT2_hoVf0M570gIRQTWDw/data-table.png" width="800"></div>

**Step 1:** <ins>Formatting Cells:</ins>

- a. Select **A1:G13**. On the **Home**, in the **Tables** group, click **Format as Table**, and choose a table style from the list. In the pop-up dialog box, ensure that the option **My table has headers**, is checked and then click **OK**.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%203%20-%20Entering%20and%20Formatting%20Data/images/2B.1a.png" width="800"></div>

- b. Select **A2:A13**. In the **Font** group click **Italic**. In the font size box, select **10**. In the font style drop-down box, select **Arial**.

**Step 2:** <ins>Formatting Cell Data:</ins>

- a. Select column **B**, and use **SHIFT+right arrow** to select across to include column **G**. On the **Home** tab, in the **Number** group, click the **Number Format** drop-down list and choose **Currency**.

- b. Select columns **B** to **G** again. On the **Home** tab, in the **Number** group, click **Decrease Decimal** once. 

- c. Select columns **B** to **G** again. On the **Home** tab, in the **Number** group, click the **Accounting Number Format ($)** drop-down list, and select **£ English (United Kingdom)**.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%203%20-%20Entering%20and%20Formatting%20Data/images/2B.2c.png" width="800"></div>

**Congratulations!**

You have completed Lab 3, and you are ready for the next topic.










