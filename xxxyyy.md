---
layout: Note
title: S1C1M3Lab1
permalink: /:title/
---

# Lab01 - Datasette Loading Data from CSV

**Estimated Time Needed: 15 Minutes**

### Overview

Now, that you have learned about the process of importing data into a data repository from varied sources, you will load data from a CSV file into the Datasette.

### Dataset

The dataset used in this exercise comes from the following source: [https://www.kaggle.com/antfarol/car-sale-advertisements](https://www.kaggle.com/antfarol/car-sale-advertisements?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDB0100ENSkillsNetwork23053252-2022-01-01) under a [CC0: Public Domain license](https://creativecommons.org/publicdomain/zero/1.0/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDB0100ENSkillsNetwork23053252-2022-01-01). 

We are using a modified subset of that dataset for this lab. To follow the lab instructions successfully, please use the dataset provided with this exercise rather than the dataset from the original source.

https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/exercise03_car_sales_data.csv is the csv file used in this lab.

### Objectives

After completing this lab, you will be able to:

- Create and Load data into a table from a CSV file.

## Exercise 1: Create a table by loading a CSV file using Datasette

In this exercise, you will learn how to load a CSV file and create a table using the Datasette tool.

**Step 1:** After launching the Datasette tool through the **Launch App** button, click on the three vertical lines located in the upper right corner to open the menu for adding datasets.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/Datasetteoptionallabs/Week3/images/menu2.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

**Step 2:** Next click the **Add DataSets** option to add the dataset.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/Datasetteoptionallabs/Week3/images/adddata.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

**Step 3:** You will be redirected to a page where you need to enter the full URL of the CSV dataset in the text box.

Right-click on the link

[exercise03_car_sales_data.csv](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/exercise03_car_sales_data.csv) and copy the link address.

Enter the copied URL in the text box and click on the create button.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/Datasetteoptionallabs/Week3/images/Data_img2.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

**Step 4:** The exercise03_car_sales_data table will be created with the data loaded from the CSV file. 

A **select** query related to the table will appear on the **text area** section of the following webpage. 

Click on the **Submit Query** button to view the results.

**Step 5:** Next, modify the **select** query as follows:

```
SELECT COUNT(*) FROM exercise03_car_sales_data;
```   

**Step 6:** Once the query executes successfully, it displays the counts.

**Congratulations!**

You have completed this lab!
