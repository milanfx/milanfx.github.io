---
layout: page
permalink: /DE03Lab02/
---

# Lab02 - Datasette Create Tables and Load Data

**Estimated Time Needed: 20 Minutes**

### Overview

In this lab, you will learn how to create tables and load data in Datasette.

### Objectives

After completing this lab, you will be able to:

- Create and load data into a table from a CSV file
- Create and load data into a table from a SQL script file

### Prerequisites

In this lab, you will use <a href="https://github.com/simonw/datasette?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDB0201ENSkillsNetwork20127838-2022-01-01" target="_blank">Datasette, </a>an open-source multi-tool for exploring and publishing data.

### Dataset

PETSHOP and BookShop are the two data sets you will use in this lab.

- PETSHOP:

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Create%20Tables%20and%20Load%20Data%20in%20Db2/images/PETSHOP_table.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

- BookShop:

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/labs/Lab%20-%20Create%20Tables%20and%20Load%20Data%20in%20Db2/images/BookShop_table.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

## Exercise 1: Load a CSV file and create a table using the Datasette tool

In this exercise, you will learn how to load a CSV file and create a table using the Datasette tool.

**Step 1:** First, select **Open tool**, then click the  **Navigation Pane** at the right-end corner, and then select **Add DataSets**.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/Datasetteoptionallabs/Week2/images/Fig1.PNG" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

**Step 2:** You will then be redirected to a page where you need to enter the full URL of the CSV data set in the text box.

Right-click the link [PETSHOP.csv](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/datasets/PET_Tables/PETSHOP.csv) and copy the link address. Enter the copied URL in the text box and select the **create** button.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/Datasetteoptionallabs/Week2/images/Fig2.PNG" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

**Step 3:** The data loaded from the CSV file will create the PETSHOP table. By default, a **SELECT** query related to the table will appear on the **text area** section of the following webpage. Click **Submit Query** to view the results.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/Datasetteoptionallabs/Week2/images/Fig3.PNG" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

**Step 4:** Next, modify the **SELECT** query as follows:

```
select count(*) from PETSHOP
```

Once you have completed this step, you should see all five rows of the PETSHOP table.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/Datasetteoptionallabs/Week2/images/Fig4.PNG" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

**Step 5:** You have successfully created and loaded the **PETSHOP** table.

## Exercise 2: Create and load data in the table using an SQL script file 

In this exercise, you will learn how to create and load data into a table by running a script containing the CREATE and INSERT SQL commands.

**Step 1:** Download the script file to your computer:

- [BookShop-CREATE-INSERT.sql](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/Datasetteoptionallabs/Week2/data/BookShop-CREATE-INSERT.sql)

**Step 2:** Open the script file using a notepad or any text editor.

Copy the contents of the script file and paste it in the datasette text area

Select Submit query

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/Datasetteoptionallabs/Week2/images/Fig5.PNG" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

**Step 3:** Next, click the **home** link at the top of the page.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/Datasetteoptionallabs/Week2/images/Fig6.PNG" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

**Step 4:** This step will redirect you to a page displaying **Databases and Tables**.

Select the **BookShop** table under the **PetShop** database.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/Datasetteoptionallabs/Week2/images/Fig7.PNG" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

**Step 5:** You will be able to view the **columns** and **data** of the **Bookshop** table.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0110EN-SkillsNetwork/Datasetteoptionallabs/Week2/images/Fig8.PNG" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

**Congratulations!**

You have completed this lab!
