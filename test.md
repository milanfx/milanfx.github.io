---
layout: page
title: Milanfx Study Notes
permalink: /xxx/
---




# Looker Getting Started

**Estimated Time Needed: 60 Minutes**

### Overview

Looker Studio, from Google, is a data discovery platform available to analyze and perform data-driven functionalities. Looker is known for its data exploration, visualization, and reporting capabilities. It empowers users to seamlessly connect with diverse data sources, enabling them to build interactive dashboards and generate insightful reports, thereby facilitating a comprehensive understanding of their data.

In this lab, you will learn how to sign up for Looker Studio and learn general navigation around the Looker user interface (UI). Next, you will learn how to upload external data files to Looker through connectors and then learn how to start a new dashboard with templates. Lastly, you will learn how to create a simple dashboard.

### Dataset

The dataset used in this lab is published by IBM. You can download the dataset file directly from here: [CustomerLoyaltyProgram.csv](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DV0130EN-SkillsNetwork/Hands-on%20Labs/Lab%204%20-%20Getting%20Started%20with%20Cognos%20Analytics/CustomerLoyaltyProgram.csv).

### Objectives

After completing this lab, you will be able to:
- Sign up to use Looker Studio
- Navigate around the Looker Studio user interface
- Create a data source using a connector
- Access report themes and layouts
- Create a simple dashboard report

## Exercise 1: Sign up for Looker Studio

In this exercise, you will learn how to sign up for Google\'s Looker Studio

**Step 1:** Go To [Looker Studio](https://lookerstudio.google.com/u/0/ "Looker Studio")

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/1_1.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 2:** Click **USE IT FOR FREE**. 

**Step 3:** A new window will open. If you already have a Google account, enter your credentials and click **Next** as shown below (number 1 and 2). Or click on **Create account** (number 3) and follow the steps.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/1_2_1.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

You are now done with the sign up procedure. You will be redirected to the Looker Studio home page automatically and your screen will appear similar to this:- <br>

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/1_3.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

## Exercise 2: Navigate around the Looker Studio User Interface

In this exercise, you will understand Looker Studio UI components which you\'ll use further to create visuals and dashboards.

The goal of this exercise is to introduce you to the primary components and functionalities within Looker Studio.

On the home page of Looker Studio, you can conveniently create and access all your essential assets, including reports, data sources, and explorations.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/2_1.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

Let\'s understand the major components available on the homepage.

**Step 1:** From here you can create a new asset such as a Report, a Data source or an Explorer. 

**Step 2:** This is where you access your recent Reports, Data sources, and Explorers.

**Step 3:** With the Report tab selected, this is how you can start to create a blank report. 

**Step 4:** This lists any recently worked on assets. You can click the ellipsis button (**...**) next to an asset to perform actions on it, such as sharing, renaming, or removing it.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/2_1_4.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 5:** Here you can search and find your Looker Studio assets quickly and the result will appear in the list at section 4.

**Step 6:** You can choose a template from the Template Gallery to start creating an asset from.

**Step 7:** Here you can take a tutorial on Looker Studio.

## Exercise 3: Create a Data Source and Use Report Editor 

### Task 1: Create a data source

The first thing you need to start creating a report is to acquire some data.

To select an existing data source you would click the **Data sources** tab and your existing data sources will be listed. 

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/3_2.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

However, for this lab, you will create a new data source.

**Step 1:** In the top left corner, click **Create**, then select **Data source**. 

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/3_3.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

The new window that opens displays a lot of options for connecting to your data; these are called *Connectors*. A connector links Looker Studio to your data. Connecting to your data creates a data source within Looker Studio. Looker Studio provides a variety of connectors to connect to different kinds of data to create reports.

You can use the search field to look for the relevant data connector.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/3_31.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/3_32.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

For this lab, you will work on  [CustomerLoyaltyProgram.csv](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DV0130EN-SkillsNetwork/Hands-on%20Labs/Lab%204%20-%20Getting%20Started%20with%20Cognos%20Analytics/CustomerLoyaltyProgram.csv)., which you need to download to your computer first. 

You will use the **File Upload** connector to upload the data to Looker Studio to create the data source.

**Step 2:** In the **Search** box, type *file upload*, then click on the **File Upload** connector. 

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/3_4.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 3:** Click the **CLICK TO UPLOAD FILES** button, select the *CustomerLoyaltyProgram.csv* file and click **Open**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/3_5.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 4:** Once the data is uploaded, click **CONNECT**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/3_6.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

Here you can see the contents of the uploaded data source. On this page you can verify or modify the data type of each data attribute, modify the default aggregation, include the description for fields, and add new fields and parameters as well.

**Step 5:** To start creating the report, click **CREATE REPORT**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/3_7.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 6:** In the pop-up dialog box, click **ADD TO REPORT**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/3_8.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

The **Report Editor** tool will open.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/3_9.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

By default, the summary table will appear as per the data source.

**Step 7:** Select the table visualization and delete it.

**Step 8:** Click the existing report title (*Untitled Report*) and rename the report to *Simple Dashboard*.

**Step 9:** To give yourself more screen space and expand the canvas window, you can close the **Data** and **Properties** panes on the right side of the page.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/3_10.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

NOTE: *To work on data in Excel format, upload the .xls file to your computer, and use the 'Google Sheets' connector to create the data source.*

### Task 2: Use Report Editor

Let\'s see what tools are available in the Report Editor.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/4_1.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 1:** To add a new chart, click **Add a chart**. Looker Studio provides a variety of charts to be used for creating visualizations such as tables, scorecards, time series charts, bar charts, line charts, pie charts, and maps to name but a few.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/4_2.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 2:** Scroll down to see all the options. To include data, click **Add data**, then close the **Add data to report** window.

**Step 3:** Click **Add a control**. Controls are used to make your visuals interactive. Looker Studio provides several control options including sliders, filters, checklists, drop-down lists, and buttons.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/4_3.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

Controls enable you to adjust the data shown in report components by filtering or modifying it. They serve as a means to collect user input and incorporate it into calculated fields.

**Step 4:** Use the icons to the right of **Add a control** to insert components other than charts and controls to your dashboard or report. These include URLs, images, textboxes, and lines and shapes. To access the **Theme and layout** option, if it is hidden, click the elipsis button (vertical three dots).

**Step 5:** The **Share** button lets you share your report with others.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/4_6.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

You can invite your colleagues to work on your dashbboard with you, you can also get the link or embedded code, and you can download the report. You also have the option to schedule the delivery time of your report.

**Step 6:** If you prefer not to make edits to the report and simply want to see how it appears in read-only mode, click **View**. You can click **Pause updates** to pause the data updates for the live data, if used, and you can refresh or make a copy of the data by clicking on the elipsis button (three vertical dots) here.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/4_7.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 7:** Click **Add page** to add more pages to your report. You can easily switch amongst pages using the left navigation bar or the arrows in the toolbar.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/4_8.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 8:** Looker Studio provides several options to zoom in and out, such as **Fit all**, **Fit width**, and various percentage values.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/4_5.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 9:** Use the **Undo** and **Redo** buttons to fix mistakes or misclicks.

**Step 10:** The main work area at position 10 is the **canvas** where you add and layout all your visualizations.

## Exercise 4: Access Report Themes and Layouts

Unlike Cognos Analytics, Looker Studio gives you the flexibity to place the visuals where you like to while you prepare the report or dashboard. So you don\'t have to select a fixed dashboard template, as you do in Cognos Analytics. However, Looker Studio does have some inbuilt themes with different color and font combinations for you to choose from. 

**Step 1:** To access the *Theme and layout* menu, either click **File** in the main menu, then click **Theme and layout**, or in the toolbar, click **Theme and layout**. If it\'s hidden, click the elipsis button (**...**) to show it. 

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/3_11.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 2:** Use the **THEME** tab to modify the default theme or select one of the predefined themes for your report. 

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/3_11_1.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 3:** Use the **LAYOUT** tab to change the layout of your canvas, such as the type of navigation, canvas size, and grid settings.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/3_11_2.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

## Exercise 5: Create a Simple Dashboard Report

Let\'s create a simple dashboard on **Product Line Performance by Year**

**Step 1:** Click **Add a chart** and select the simple **Line chart**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/5_2.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 2:** Click on the canvas where you want it to be positioned. You can move it anywhere on the canvas later by simply clicking and dragging it to a new position. Looker Studio automatically includes data to create the chart based on the data source.

For your *Product Line Performance by Year* visualization, you place the data as you want it to be displayed. The requirement is to create a line chart for the quantity sold per order year and have separate lines displayed for each product line.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/5_1.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 3:** Click on the line chart in the canvas, and then click **Properties**.

**Step 4:** Click **Data** to open that pane on the right too.

**Step 5:** From the data pane, drag **Order Year** to the **Dimension** field to replace **First Name**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/5_3.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 6:** From the data pane, drag **Quantity Sold** to the **Metric** field. Remove the **Record Count** item.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/5_4.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

You want to break down the chart by product line, so that it can display a separate line for each product category.

**Step 7:** From the data pane, drag **Product Line** to the **Breakdown dimension** field.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/5_5.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 8:** To include the x and y axis labels, click the **STYLE** tab in the chart\'s **Properties** pane, and check the box for **Show axis title** in both the **Left Y-axis** and the **X-axis** sections.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/5_11.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 9:** Hover over the bottom right corner of the chart till you see the white double-headed arrow, then click and drag to make the chart larger.

**Step 10:** In the main toolbar, select the **Text** tool and click above the visualization to insert a text box for the chart title. Click in the text box and type the title as *Product Line Performance by Year*. 

**Step 11:** Select the text in the new title and use the **Text Properties** in the right pane to style the text as **24pt**, **bold**, and **dark blue**. 

**Step 12:** Drag the text box to align it with the center of the line chart visualization, and drag the chart and the title boxes down the page a bit to make some room at the top for the next visualization. 

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/5_6.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

Your line chart should now look similar to the image below.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/5_7_1.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

Now you will include two scorecards to display the *Total Quantity Sold* and *Revenue* above this line chart.

**Step 13:** In the toolbar, click **Add a chart**, and select **Scorecard**.

**Step 14:** Move it above the line chart visualization and to the left side of the canvas. 

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/5_8.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

Looker Studio will automatically pick **Quantity Sold** to be displayed on this scorecard. 

**Step 15:** You can change the size and position as you like. 

**Step 16:** Use the **STYLE** tab in the scorecard chart\'s **Properties** pane to change the font size and color to **48pt** and **dark blue**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/5_9.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

Now you will add the second scorecard chart above the line chart.

**Step 17:** In the toolbar, click **Add a chart**, and select **Scorecard**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/5_8.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 18:** Place it to the right of the **Quantity Sold** scorecard chart. 

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/5_10.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

This time Looker Studio has picked **Record Count** to create this scorecard. 

Let\'s change the metric to show *Revenue* instead.

**Step 19:** Select the **SETUP** tab in the scorecard chart\'s **Properties** pane.

**Step 20:** From the **Data** pane, drag **Revenue** to the **Metric** field to replace **Record Count**.

**Step 20:** Use the **STYLE** tab in the scorecard chart\'s **Properties** pane to change the font size and color to **48pt** and **dark blue** as you did for the previous scorecard chart.

The final version of your first dashboard should appear similar to the image below.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/5_12.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Congratulations!**

You have completed this lab!



