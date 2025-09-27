---
layout: page
title: Milanfx Study Notes
permalink: /xxx/
---


# Db2 Explore Your Dataset Using SQL Queries

**Estimated Time Needed: 15 Minutes**

## Overview

Now that you have learned how querying techniques can help you to explore and analyze your data, you will run some basic SQL queries on the data you loaded into your database instance in the previous lab. For this, you will use the in-built SQL editor available in your Lite account.

---

# Practice

Please follow the steps given below to explore your dataset using SQL queries.

1.  Click on [https://cloud.ibm.com/catalog/services/db2](https://cloud.ibm.com/catalog/services/db2?utm_source=skills_network&utm_content=in_lab_content_link&utm_id=Lab-IBM-DB0100EN-SkillsNetwork) to access your Db2 dashboard on Cloud.

2.  If you’re not already logged in to your IBM Cloud Lite account, click on **Log in** at the bottom right of the screen to log in.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_4-1.png" width="25%"><br> 

3.  Logging in will take you to your **Db2 service dashboard**.

Click on **view existing** link in the **Existing Lite plan instance** box.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_4-2.png" width="50%"><br> 

4.  The **Manage** tab will be active by default in your services dashboard. Click on the **Go to UI** button.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_4-3.png" width="50%"><br> 

5.  Click on the 3-bar menu at the top left of the screen and select **RUN SQL** from the dropdown menu.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_4-4.png" width="50%"><br> 

6.  On the next screen click on **Create new**.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_4-5.png" width="50%"><br> 

7.  The **SQL editor** will open.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_4-6.png" width="50%"><br> 

8.  Click on the highlighted row and copy-paste the following query into the highlighted row.

select count(*) from CARSALESTABLE;

Click on **Run all** at the bottom left of the screen to run the query.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_4-7.png" width="75%"><br> 

9.  Close the Result Set window and then copy and paste the following query into the **SQL editor**, replacing the existing query text.

select max(price) as max_price from CARSALESTABLE;

Click on **Run all** at the bottom left of the screen to run the query.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_4-9.png" width="75%"><br> 

10.  Click on the **arrow** <img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_7A.png" width="50"> on the right side of the screen to view the result of your query.

A pop-window will open with the result.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_4-10.png" width="25%"><br> 

11.  Close the Result Set window and then copy and paste the following query into the **SQL editor**, replacing the existing query text.

select distinct(model) from CARSALESTABLE;

Click on **Run all** at the bottom left of the screen to run the query.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_4-11.png" width="75%"><br> 

**Congratulations!** 

You have successfully run some SQL queries to help you explore and understand your dataset.


