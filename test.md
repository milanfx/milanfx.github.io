---
layout: page
title: Milanfx Study Notes
permalink: /xxx/
---


# Excel Multiple Linear Regression Analysis

**Estimated Time Needed: 30 Minutes**

### Overview

In this lab, you\'ll learn how to perform a multiple linear regression analysis using Microsoft Excel.

### Software

The instruction videos in this course will be using the full Excel Desktop version because it has all the available product features. However, for the hands-on labs, we will use the free \"Excel for the web\" version because this is available to everyone.

Although you can use the Excel Desktop software, <a href="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%201%20-%20Access%20to%20the%20environment%20-%20Excel%20for%20the%20web/instructions.md.html">it is recommended that you use Excel for the web for the hands-on labs</a>, as the lab instructions specifically refer to this version. There are some small differences in the interface and available features.

### Dataset

The data set used in this lab is curated from the following source: https://www.kaggle.com/datasets/yasserh/housing-prices-dataset under the [CC0: Public Domain](https://creativecommons.org/publicdomain/zero/1.0/ "CC0: Public Domain license") license.

Acknowledgment and thanks also go to https://trak.in, who were generous enough to share the data publicly for free.

**NOTE:** We are using a modified subset of the original data set. Please ensure you use the data set provided in this lab.

#### Learning objectives:

- Perform a multiple linear regression analysis.
- Assess how well the regression equation predicts the dependent variable.
- Assess the contribution of each independent variable to the prediction.

Welcome to the Lab: Multiple Linear Regression Analysis!

## Configure the XL Miner Analysis ToolPak

Before you begin with the lab, let\'s configure the XL Miner Analysis ToolPak in your Excel for the web version. You will need this add-in to perform the regression analysis. If you have already configured the add-in, you may skip this section.

**NOTE:** XLMiner Analysis ToolPak is a third-party free statistical analysis ToolPak in Excel for the web. It shows the same functions as the Analysis ToolPak add-in available in Excel for the desktop. You can use this ToolPak to perform descriptive statistics and linear regression for the labs in this course. If you are using Excel for the desktop, you can configure the in-built Data Analysis ToolPak available from Microsoft. 

To configure this add-in, open a file in Excel for the web and follow the following steps.

**Step 1:** Select **File** on the top ribbon.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/images/Rev_Img_1.png" style="width:880px; max-height:600px; object-fit:contain;"></div></div>

**Step 2:** Select Get **Add-ins** from the left menu bar and choose **More Add-ins**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/images/Rev_Img_2.png" style="width:880px; max-height:600px; object-fit:contain;"></div></div>

**Step 3:** In the **Office Add-ins** window, type in **Analysis ToolPak** in the search bar and select the search icon. 

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/images/Rev_Img_3.png" style="width:880px; max-height:600px; object-fit:contain;"></div></div>

**Step 4:** Select the **Add** button next to the **XLMiner Analysis ToolPak**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/images/Rev_Img_4.png" style="width:880px; max-height:600px; object-fit:contain;"></div></div>

**Step 5:** Select the checkbox next to **I agree to all the above terms & conditions**. Select **Continue**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/images/Rev_Img_5.png" style="width:880px; max-height:600px; object-fit:contain;"></div></div>

**Step 6:** You\'ll see **XLMiner Analysis ToolPak** on the right side of your Excel sheet. You\'ll also see the **Show ToolPak** button in the ribbon.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/images/Rev_Img_6.png" style="width:880px; max-height:600px; object-fit:contain;"></div></div>

## Exercise: Perform a multiple linear regression analysis to predict the test score

In this exercise, you\'ll learn to identify dependent and independent variables, perform multiple linear regression, evaluate the regression model, and assess the contribution of each independent variable.

For this lab, you will use the following data set, [Lab_Multiple Linear Regression_Data set.xlsx](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/Lab_Multiple%20Linear_Regression_Data_set.xlsx "Lab_Multiple Linear Regression_Data set.xlsx"). To download the data set, right-click the hyperlink and select Open link in a new tab. Open the file in Excel for the Web version and follow the steps given below to perform the regression analysis.

Here\'s a screenshot of the data set.
<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/images/1_MLRA.png" style="width:880px; max-height:600px; object-fit:contain;"></div></div>

### Task 1: Identify the dependent and independent variables
In this task, you\'ll predict the house prices, which depend on three variables: the area of the house in square feet, the inflation rate, and the bank\'s rate of interest. Thus, house prices are the dependent variable, whereas the area of the house in square feet, the inflation rate, and the bank\'s rate of interest are the independent variables.

You will use the following multiple regression equation with three independent variables:

Y = β<sub>0</sub> + β<sub>1</sub>X<sub>1</sub> + β<sub>2</sub>X<sub>2</sub> + β<sub>3</sub>X<sub>3</sub>
 
Where

- Y: House price (Dependent variable)
- X<sub>1</sub>: Area of the house in square feet (Independent variable)
- X<sub>2</sub>: The inflation rate (Independent variable)
- X<sub>3</sub>: The interest rate (Independent variable)
- β<sub>0</sub>: The y-intercept
- β<sub>1</sub>, β<sub>2</sub>, and β<sub>3</sub>: The slope coefficients

### Task 2: Perform the multiple linear regression

In this task, you\'ll perform regression analysis using Excel. 

**Step 1:** You\'ll be using the XL Miner Analysis Toolpak to perform this task. To open the add-in, Click the **Show ToolPak** icon within the **Home** tab. 

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/images/2_MLRA.png" style="width:880px; max-height:600px; object-fit:contain;"></div></div>

**Step 2:** The **XLMiner Analysis ToolPak** will appear. Select **Linear Regression**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/images/3_MLRA.png" style="width:880px; max-height:600px; object-fit:contain;"></div></div>

**Step 3:** Populate the regression analysis fields with the below range.

- **Input Y Range:** The housing prices **($E$1:$E$12)**.
- **Input X Range:** Area in square feet, the inflation rate, and the bank\'s rate of interest **($B$1:$D$12)**.
- Select the **Labels** checkbox.
- Uncheck **Confidence Level**.
- **Output Range:** $H$1
- Select **OK**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/images/4_MLRA.png" style="width:880px; max-height:600px; object-fit:contain;"></div></div>

**Step 4:** The regression analysis results will appear. 

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/images/5_MLRA.png" style="width:880px; max-height:600px; object-fit:contain;"></div></div>

**Step 5:** The regression output shows the coefficients. You can thus determine the regression equation as follows: 

Y = β<sub>0</sub> + β<sub>1</sub>X<sub>1</sub> + β<sub>2</sub>X<sub>2</sub> + β<sub>3</sub>X<sub>3</sub>

Y = -483410.67 + 261.05X<sub>1</sub> + 95473.76X<sub>2</sub> + 147274.52 X<sub>3</sub>

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/images/6_MLRA.png" style="width:880px; max-height:600px; object-fit:contain;"></div></div>

### Task 3: Evaluate the model

Next, you\'ll evaluate the regression model by examining some of the values in this analysis summary.

**Step 1:** Examine the **R-squared value**. The R-squared value for the given data set is 0.93. This means that the independent variables, the area in square feet, the inflation rate, and the bank\'s rate of interest, are collectively responsible for 93% of the variance in the house price. 

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/images/7_MLRA.png" style="width:880px; max-height:600px; object-fit:contain;"></div></div>

**Step 2:** Next, assess the statistical significance of the regression sum of squares. Examine the ANOVA table produced for the given data set using Excel. 
This table shows the **F-statistic** and the **Significance F** value. The F-statistic value is 33.17, which is a high value, and the model\'s p-value or Significance F is 0.000165, which is less than 0.05. This indicates that one or all of the independent variables have explanatory power beyond what would be expected by chance. 

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/images/9_MLRA.png" style="width:880px; max-height:600px; object-fit:contain;"></div></div>

**Step 3:** To assess the contribution of each independent variable, examine their **p-values**. The p-values for the area in square feet is 0.0022, the bank\'s rate of interest is 0.16, and that of the inflation rate is 0.09. A low p-value, typically less than 0.05, indicates that the corresponding regression coefficient is statistically significant, implying that the independent variable has a meaningful impact on the dependent variable.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-ST0141EN-Coursera/images/10_MLRA.png" style="width:880px; max-height:600px; object-fit:contain;"></div></div>

**Congratulations!**

You have completed this lab!







