---
layout: page
title: Milanfx Study Notes
permalink: /xxx/
---



# Excel Measure of Dispersion
	
**Estimated Time Needed: 30 Minutes**

### Overview

In this lab, you will learn to calculate the measure of dispersion and describe the spread or dispersion in the data. Next, you will learn about the different types of measurement of dispersion with the help of real-life examples. You will also be able to calculate a range, quartile range, variance, and standard deviation for the given data set using Excel.

### Software Used in this Lab

The instruction videos in this course use the full Excel Desktop version as this has all the available product features, but for the hands-on labs, we will be using the free "Excel for the web" version as this is available to everyone.

Although you can use the Excel Desktop software if you have access to this version, <a href="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%201%20-%20Access%20to%20the%20environment%20-%20Excel%20for%20the%20web/instructions.md.html">it is recommended that you use Excel for the web for the hands-on labs</a>, as the lab instructions specifically refer to this version, and there are some small differences in the interface and available features.

### Data set Used in this Lab

The data set used in this lab is curated from the following source: https://www.kaggle.com/datasets/anandaramg/nyc-jobs-openings-2022 under the [CC0: Public Domain](https://creativecommons.org/publicdomain/zero/1.0/ "CC0: Public Domain") license.

Acknowledgment and thanks also go to https://trak.in who were generous enough to share the data publicly for free.

We are using a modified subset of that data set for the lab, so to follow the lab instructions successfully, please use the data set provided in this lab rather than the data set from the original source.

### Learning Objectives:

- Describe types of measurement of dispersion
- Calculate range, variance, and standard deviation using Excel
- Implement Excel formulas of range, variance, and standard deviation to find dispersion for the given data sets

Welcome to the Lab: Measure of Dispersion!

## Exercise: Calculate the Measurement of Dispersion using the Range, Variance, and Standard Deviation

In this exercise, you\'ll learn to calculate range, variance, and standard deviation for the measurement of dispersion using Excel for the web. You will also learn that the dispersion or variability measures can describe the data\'s spread or dispersion using Excel for the web. You can follow the tasks below to perform this exercise.

### Task A: Calculate Average

**Step 1:** To calculate the average, use a data set for which you want to find the average. In this case, let\'s use the data set of [job openings in the years 2022 and 2023](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/Mz4niWqEW7nPCOI_0JLNwg/Lab-M1-Lab1-Measure-of-Dispersion.xlsx "job openings in the years 2022 and 2023") (To download the given data set in this lab, right click on the given hyperlink and select Open link in new tab) for business intelligence (BI) roles.

|  Number of job openings |2022 | 2023 |
| ------------ | ------------ | ------------ |
| Data scientist  | 8500 | 9800  |
| Data engineer  | 4500 | 6400 |
| Python developer | 8400 | 5600 |
| Cyber security expert | 1000 | 900  |

**Step 2:** Copy or transfer the given data set in Excel.

<div style="display: inline-grid; border: 3px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/Measure_of_Dispersion/1.png" width="800"></div>

Let\'s first calculate the average using either of the following two methods:

Method 1: Calculate the average from the **Formulas** tab in Excel.

Method 2: Apply the **Average** formula to the given data set in Excel.

### Method 1: Calculate the Average from the Formulas tab in Excel

**Step 1:** To calculate the average job openings in the year 2022, select the data column you want to find the average.

<div style="display: inline-grid; border: 3px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/Measure_of_Dispersion/2.png" width="800"></div>

**Step 2:** Select the **Formulas** tab and choose **AutoSum** from the ribbon. A drop-down list will appear.

<div style="display: inline-grid; border: 3px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/Measure_of_Dispersion/3.png" width="800"></div>

**Step 3:** From the  drop-down list, select **Average**. You can see that the **Average** value is calculated for job openings in the year 2022. You\'ll  get the value 5600.

<div style="display: inline-grid; border: 3px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/Measure_of_Dispersion/4.png" width="800"></div>

### Method 2: Apply the Average formula in Excel

**Step 1:** Now, let\'s calculate the **Average** for job openings in the year 2023 using the Average formula. To do so, type in the formula **=Average()** below job openings in the 2023 column and select the data range for which you want to calculate the average.

**Step 2:** Press **Enter** to get the average value for the job openings in the year 2023. You\'ll get the value 5675.

<div style="display: inline-grid; border: 3px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/Measure_of_Dispersion/5.png" width="800"></div>

### Task B: Calculate the Range

You can calculate the range for the data by subtracting the minimum value from the maximum value using the Excel formula **=MAX()–MIN()**. However, the formula =MAX() helps to find the maximum value, and the formula =MIN() helps to find the minimum value for the data set in Excel for the web. Perform the following steps to calculate the range in Excel for the web.

**Step 1:** To calculate the maximum value in the given data set for the job openings in the year 2022, type in the formula **=MAX()** and select the range for the data column. Next, press **Enter** to get the maximum value. You\'ll get a maximum value 8500.

<div style="display: inline-grid; border: 3px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/Measure_of_Dispersion/6.png" width="800"></div>

**Step 2:** To calculate the minimum value in the given data set for job openings in the year 2023, type in the formula **=MIN()** and select the range for the data column. Next, press **Enter** to get the minimum value. You\'ll get a minimum value 900.

<div style="display: inline-grid; border: 3px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/Measure_of_Dispersion/7.png" width="800"></div>

**Step 3:** To calculate the range for the job opening in the year 2022, type in the formula **=MAX()–MIN()**. Press **Enter** to get the value for Range. You will get a value as 7500. In a similar way, you can calculate the range for the job openings for the year 2023.

<div style="display: inline-grid; border: 3px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/Measure_of_Dispersion/8.png" width="800"></div>

### Quartile Function

Now, let\'s look at the quartile function.

Quartile functions are of two types: Inclusive quartile function and exclusive quartile function. Both functions calculate the quartile by calculating the percentage of the data.

### Inclusive Quartile Function

The inclusive quartile function is a difference between the quartile 3 and quartile 1 values. It also includes the quartiles 0 and 4 to calculate the values of quartiles. Let\'s calculate an inclusive quartile value for the job openings in the year 2022 for the given data set.

**Step 1:** To calculate the inclusive quartile for quarter 3, type in the formula **=QUARTILE.INC**, select a range for the job openings in the year 2022 and insert comma 3. Next, press **Enter**. You\'ll get the value for the inclusive quartile for quarter 3 as 8425.

<div style="display: inline-grid; border: 3px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/Measure_of_Dispersion/9.png" width="800"></div>

**Step 2:** Now, let\'s calculate the inclusive quartile for quarter 1 for the job openings in the year 2023. To do so, type in the formula **=QUARTILE.INC**, select the range for the job openings in the year 2023 and insert comma 1. Next, press **Enter**. You\'ll get the value for the inclusive quartile for quarter 1 as 4425.

<div style="display: inline-grid; border: 3px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/Measure_of_Dispersion/10.png" width="800"></div>

**Step 3:** To calculate the inclusive interquartile range, use the minus formula in Excel for Quartile 3 and Quartile 1. Press **Enter**. You\'ll get the interquartile range 4800 and 2825 for the job openings in the year 2022 and 2023, respectively.
<div style="display: inline-grid; border: 3px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/Measure_of_Dispersion/11.png" width="800"></div>

### Exclusive Quartile Function

The exclusive quartile range function cannot calculate quartile 0 or quartile 4. It means that it excludes extreme values. Let\'s calculate an exclusive quartile value for the given data set.

**Step 1:** To calculate the exclusive quartile quarter 3 for the job opening in the year 2022, type in the formula **=QUARTILE.EXC**, select the range for the job opening in the year 2022 and insert comma 3. Next, press **Enter**. You\'ll get the value 8475.

<div style="display: inline-grid; border: 3px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/Measure_of_Dispersion/12.png" width="800"></div>

**Step 2:** In a similar way, to calculate the exclusive quartile value for quarter 1 for the job openings in the year 2023, type in the formula **=QUARTILE.EXC**, select a range for the year 2023 and insert comma 1. Press **Enter**. You\'ll get the value 2075.

<div style="display: inline-grid; border: 3px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/Measure_of_Dispersion/13.png" width="800"></div>

**Step 3:** To calculate the exclusive interquartile range, use the minus formula in Excel for Quartile 3 and Quartile 1. Press **Enter**. You\'ll get the interquartile range 6600 and 6875 for the job openings in the year 2022 and 2023, respectively.

<div style="display: inline-grid; border: 3px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/Measure_of_Dispersion/14.png" width="800"></div>

### Task C: Calculate the Variance

Variance is the average of the squared deviations and measures the distance from the mean or average for each data in the data set. Variance calculations depend on whether the data set describes the sample or the entire population. Let\'s review these two types of variances.

### Calculate Population Variance

**Step 1:** To calculate the population variance, you\'ll use the same data set for job openings in the year 2022 and 2023. You can manually calculate variance by dividing the squared deviations sum by \'n.\'

**Step 2:** Let\'s first calculate the population variance for the job opening in the year 2022 using Excel. To do so, type in the formula **=VAR.P()** and select the range for the job opening in the year 2022. Press **Enter**. You\'ll get a value of 965,5000.

<div style="display: inline-grid; border: 3px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/Measure_of_Dispersion/15.png" width="800"></div>

### Calculate Sample Variance

**Step 1:** To calculate the sample variance, use the given data set of job openings in the years 2022 and 2023. You can manually calculate variance by dividing the squared deviations sum by \'(n − 1)\'.

**Step 2:** Now, let\'s calculate the sample variance for the job openings in the year 2023 using Excel. To do so, type in the formula **=VAR.S()** and select the range for the job openings in the year 2023. Press **Enter**. You\'ll get a value 134,491,66.67.
<div style="display: inline-grid; border: 3px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/Measure_of_Dispersion/16.png" width="800"></div>

### Task 4: Calculate the Standard Deviation

Standard deviation is the square root of variance. However, the standard deviation can also differ if the calculated variance differs for the population and the sample variance. You can calculate the standard deviation using the equation,

<div style="display: inline-grid; border: 3px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/images/Formula1.png" width="800"></div>

Where

- *x<sub>i</sub>* = Each value in the data set
- *x&#772;* = Mean of all values in the data set
- *N* = Number of values in the data set

Excel provides two functions for the standard deviation: Population and sample. Let\'s perform the steps to calculate the standard deviation using Excel.

**Step 1:** To calculate the population standard deviation for the job openings in the year 2022, use the Excel formula **=STDEV.P()** and select the range for the data set.

**Step 2:** Next, press **Enter**. You\'ll get a value 3107.25.

<div style="display: inline-grid; border: 3px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/Measure_of_Dispersion/17.png" width="800"></div>

**Step 3:** To calculate the sample standard deviation for the job openings in the year 2023, use the Excel formula **=STDEV.S()** and select the range for the data set. Then, press Enter to get the value for the sample standard deviation. You\'ll get the value 3667.31.

<div style="display: inline-grid; border: 3px solid Gray;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/Measure_of_Dispersion/18.png" width="800"></div>

**Congratulations!**

You\'ve completed lab activity measure of dispersion, and you are ready to move to the next topic.







