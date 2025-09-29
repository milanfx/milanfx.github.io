---
layout: page
title: Milanfx Study Notes
permalink: /xxx/
---



# Excel Using Pivot Tables

**Estimated Time Needed: 30 Minutes**

### Overview

In this lab, first you will learn how to format data as a table, how to create a Pivot Table and use fields to arrange data in a Pivot Table, and how to perform calculations using Pivot Table data. Next, you will learn some other features that we can use with Pivot Tables, including Recommended Charts, Filters, Slicers, and Timelines.

### Software Used in this Lab

The instruction videos in this course use the full Excel Desktop version as this has all the available product features, but for the hands-on labs we will be using the free 'Excel for the web' version as this is available to everyone.

Although you can use the Excel Desktop software if you have access to this version, <ins>it is recommended that you use Excel for the web for the hands-on labs</ins> as the lab instructions specifically refer to this version, and there are some small differences in the interface and available features.

### Dataset Used in this Lab

The dataset used in this lab comes from the following source: https://www.kaggle.com/sudalairajkumar/indian-startup-funding under a **[CC0: Public Domain license](https://creativecommons.org/publicdomain/zero/1.0/)**. 
Acknowledgement and thanks also goes to https://trak.in who were generous enough to share the data publicly for free.

We are using a modified subset of that dataset for the lab, so to follow the lab instructions successfully please use the dataset provided with the lab, rather than the dataset from the original source.

### Objectives

After completing this lab, you will be able to:

- Format data as a table
- Create a Pivot Table and use fields to arrange data in a Pivot Table
- Perform calculations using Pivot Table data
- Use the Recommended Charts feature (does not work with the 'Basic' Office for the web plan.)
- Use the Filters feature
- Use the Slicers feature
- Use the Timelines feature 

## Exercise 1: Introduction to Creating Pivot Tables in Excel

In this exercise, you will learn how to format data as a table, how to create a Pivot Table and use fields to arrange data in a Pivot Table, and how to perform calculations using Pivot Table data.

### Task A: Format data as a table

**Step 1:** Download the file **[indian_startup_funding_Lab7.xlsx](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%207%20-%20Using%20Pivot%20Tables/indian_startup_funding_Lab7.xlsx)**. Upload and open it using Excel for the web.

**Step 2:** Select cell **A2**.

**Step 3:** On the **Home** tab, in the **Tables** group, click **Format as Table**.

**Step 4:** Select **Light Gray, Table Style Medium 15**.

### Task B: Create a pivot table and use fields to arrange data in a pivot table

**Step 1:** Select cell **D4**

**Step 2:** On the **Insert** tab, click **PivotTable**.

**Step 3:** Click **OK**.

<div style="text-align: center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%207%20-%20Using%20Pivot%20Tables/images/1.B.3.png" width="400"></div>

**Step 4:** Double-click **Sheet1**, type **Pivot1** and click **OK**.

**Step 5:** In the fields list, drag **Industry Vertical** to **Rows**.

**Step 6:** In the fields list, drag **City Location** to **Rows** above **Industry Vertical**.

**Step 7:** In the fields list, drag **Startup Name** to **Rows** below **Industry Vertical**.

**Step 8:** In the fields list, drag **Amount in USD** to **Values**.

**Step 9:** Use the drop down arrow for the **City Location** and Sort By Value  in descending order (Largest to smallest) by the **Count of Amount in USD**.

<div style="text-align: center; border: 1px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/images/sorting1.png" width="400"></div> 

<div style="text-align: center; border: 1px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/images/sorting2.png" width="400"></div>

**Step 10:** In the ribbon, select the **PivotTable** tab, click **Settings**, then in the **PivotTable Settings** pane, under **Layout**, select **Single column**.

**Step 11:** Right-click on the row label Amritsar and select **Expand/Collapse** and **Collapse Entire Field**. 

<div style="text-align: center; border: 1px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/images/collapse.png" width="600"></div>

### Task C: Perform a simple calculation in a pivot table

**Step 1:** In the **PivotTable Fields** pane, in the **Values** section, click the drop-down arrow next to **Count of Amount in USD**, and click **Value Field Settings**.

**Step 2:** Select **Summarize value field by > Sum**.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%207%20-%20Using%20Pivot%20Tables/images/1.C.2.png" width="400"></div>

**Step 3:** Click **OK**.

**Step 4:** Select the column called **Sum of Amount in USD** and then on the **Home** tab, select **Accounting Number Format > $ English (United States)**.

## Exercise 2: Pivot Table Features

In this exercise, you will learn some other features that we can use with Pivot Tables, including Recommended Charts, Filters, Slicers, and Timelines.

**NOTE:** The 'Recommended Charts' feature only works with 'full' Office for the web plans (those plans that come with an Office 365 subscription). Recommended Charts do not work with the 'basic' plan that comes with a Microsoft Account.

### Task A: Use of the Recommended Charts feature (Optional: If you have a full Office for the web plan)

**Step 1:** Switch to worksheet **indian-startup-funding**.

**Step 2:** Select column **F (City Location)**.

**Step 3:** On the **Insert** tab, select **Recommended Charts**.

**Step 4:** Click **+ Insert PivotChart**.

<div style="text-align: center; border: 1px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%207%20-%20Using%20Pivot%20Tables/images/2.A.4.png" width="600"></div>

**Step 5:** Switch to worksheet **indian-startup-funding** again.

**Step 6:** Select column **C, D, E**.

**Step 7:** On the **Insert** tab, select **Recommended Charts**.

**Step 8:** Choose the recommended chart, and click **+ Insert PivotChart**.

<div style="text-align: center; border: 1px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%207%20-%20Using%20Pivot%20Tables/images/recommend1.png" width="600"></div>

### Task B: Use of the Filters feature

**Step 1:** Switch to worksheet **Pivot1**.

**Step 2:** In the Pivot Table, click the **Row Labels** arrow.

**Step 3:** Select **City Location**, then **Filter...**.

**Step 4:** Just select **Burnsville**, **Delhi**, **New York**, then click **OK** to display the amounts for startups in these three cities only.

**Step 5:** In the Pivot Table, click the **Row Labels** arrow.

**Step 6:** Select **City Location**, then click **Clear Filter From 'City Location'** to display the startups in all cities again.

### Task C: Use of the Slicers feature

**Step 1:** Download the file **[indian_startup_funding_Lab7_with_slicers_timelines.xlsx](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%207%20-%20Using%20Pivot%20Tables/indian_startup_funding_Lab7_with_slicers_timelines.xlsx)**. Upload and open it using Excel for the web.

**Step 2:** Switch to worksheet **Pivot1** if you are not there.

**Step 3:** In the **City Location** slicer, select **Burnsville**, then **Delhi**, then **New York**.

**Step 4:** To filter by multiple selection in the **City Location** slicer, with **New York** still selected, press **CTRL** and select **Burnsville**, and then **Delhi**.

**Step 5:** To filter using more than one slicer, in the **Investors Name** slicer, select **Amour Infrastructure**, then press **CTRL** and select **Westbridge Capital**, and then **Breakthrough Energy Ventures**.

**Step 6:** In the **City Location** slicer, click the **Clear Filter** button, then in the **Investors Name** slicer, click the **Clear Filter** button.

### Task D: Use of the Timelines feature

**Step 1:** In the Date timeline, click **top right drop-down** and select **DAYS**, then scroll **left and right**.

<div style="text-align: center; border: 1px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%207%20-%20Using%20Pivot%20Tables/images/2.D.1.png" width="600"></div>

**Step 2:** In the Date timeline, click **top right drop-down** and select **QUARTERS**.

**Step 3:** In the Date Timeline, select **2019 Q1**, then drag **2019 Q1 to 2019 Q3**.

**Step 4:** In the Date timeline, click the **Clear Filter** icon.

**Step 5:** In the Date timeline, click **top right drop-down** and select **YEARS**, then select **2020** only.

**Congratulations!**

You have completed Lab 7, and you are ready for the next topic.











