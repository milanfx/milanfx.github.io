---
layout: page
title: Milanfx Study Notes
permalink: /xxx/
---


# Db2 Load Data from a CSV file

**Estimated Time Needed: 15 Minutes**

### Overview

Now that you have learned about the process of importing data into a data repository from varied sources, you will load data from a CSV file into the IBM Db2 database instance you created in the previous lab.

### Datasets

The dataset used in this exercise comes from the following source: [https://www.kaggle.com/antfarol/car-sale-advertisements](https://www.kaggle.com/antfarol/car-sale-advertisements) under a [CC0: Public Domain license](https://creativecommons.org/publicdomain/zero/1.0/). We are using a modified subset of that dataset for this lab. To follow the lab instructions successfully, please use the dataset provided with this exercise rather than the dataset from the original source.

**NOTE:** The lab assumes that you have downloaded this CSV file: [exercise03_car_sales_data.csv](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/exercise03_car_sales_data.csv) to your local system.

## Practice

Please follow the steps given below to provision your instance of IBM Db2 on Cloud.

**Step 1:**  Go to: [https://cloud.ibm.com/catalog/services/db2](https://cloud.ibm.com/catalog/services/db2?utm_source=skills_network&utm_content=in_lab_content_link&utm_id=Lab-IBM-DB0100EN-SkillsNetwork) to access your Db2 dashboard on Cloud.
**Step 2:**  If you’re not already logged in to your IBM Cloud Lite account, click on **Log in** at the bottom right of the screen to log in.

<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-1.png" style="width:880px; max-height:500px; object-fit:contain;"></div><br>

**Step 3:**  Logging in will take you to your **Db2 service dashboard**.

Click on **view existing** link in the **Existing Lite plan instance** box.

<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-2.png" style="width:880px; max-height:500px; object-fit:contain;"></div><br> 

**Step 4:**  The **Manage** tab will be active by default in your services dashboard. Click on **Go to UI**.

<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-3.png" style="width:880px; max-height:500px; object-fit:contain;"></div><br> 

**Step 5:**  Now click on the menu bar icon in the top left corner of your Db2 service dashboard.

Click on **Load** **>** **Load Data**.

<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-4.png" style="width:880px; max-height:500px; object-fit:contain;"></div><br> 

**Step 6:**  You can either drag and drop the CSV file into the **File selection** box, or you can click on the **browse files** link, also provided in the **File selection** box to browse your local folders to find and open the downloaded CSV file.

<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-5.png" style="width:880px; max-height:500px; object-fit:contain;"></div><br> 

The name of the CSV file you have uploaded will appear in the **Selected file** section on the right.

<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-6.png" style="width:880px; max-height:500px; object-fit:contain;"></div><br> 

Click **Next** to proceed.

**Step 7:**  You will be asked to select a **Schema** from a list of schema names.

**NOTE:** Select the schema name with a random mix of alphabets and numbers. It will be similar to, but not the same as, the one you see in the screenshot below (_MGJ73335_). The ones that you do NOT have to select are AUDIT, DB2INST1, ERRORSCHEMA, and ST_INFORMTN_SCHEMA (and sometimes you might also see SQLxxxxx as well).

<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-7.png" style="width:880px; max-height:500px; object-fit:contain;"></div><br>
**Step 8:**  Click on **New Table**.

<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-8.png" style="width:880px; max-height:500px; object-fit:contain;"></div><br> 

**Step 9:**  Enter the name **CARSALESTABLE** in the input box prompting you with **_NEW TABLE NAME_**.

**NOTE:** You will be using this table name in the SQL queries you will execute in the next exercise.

Now click on **Create** to create the new table.

<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-9.png" style="width:880px; max-height:500px; object-fit:contain;"></div><br> 

**Step 10:**  A table by the name of **CARSALESTABLE** has been created.

Click **Next** at the bottom right of the page to proceed.

<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-10.png" style="width:880px; max-height:500px; object-fit:contain;"></div><br> 

**Step 11:**  Click **Next** to proceed.

<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-11.png" style="width:880px; max-height:500px; object-fit:contain;"></div><br>

**Step 12:**  Then click **Begin Load** to begin the process of loading the data from the CSV into your database.

<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-12.png" style="width:880px; max-height:500px; object-fit:contain;"></div><br> 

**Step 13:**  Data from your CSV file is now loaded into your Db2 instance.

<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-13.png" style="width:880px; max-height:500px; object-fit:contain;"></div><br> 

**Congratulations!** 

You have successfully loaded data from a CSV file into the IBM Db2 instance you created in the previous lab.





