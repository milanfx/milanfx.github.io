---
layout: page
title: Milanfx Study Notes
permalink: /xxx/
---



# Cognos Advanced Dashboard Capabilities

**Estimated Time Needed: 45 Minutes**

### Purpose of the Lab: 

This lab focuses on enhancing skills in utilizing advanced features of IBM Cognos Analytics to create more dynamic and interactive dashboards. It delves into creating calculations, manipulating data points within visualizations, applying top/bottom settings on visualizations, and constructing navigation paths. Additionally, the lab provides hands-on experience in filtering data within a dashboard. The exercises are designed to provide a deeper understanding of how to leverage Cognos Analytics for more complex data analysis and visualization tasks, moving beyond basic dashboard creation. 

### Benefits of Learning the Lab: 

Engaging in this lab offers several key benefits for those interested in data analytics and visualization.You will acquire practical skills in advanced dashboarding techniques, such as creating custom calculations, effectively filtering and manipulating data, and utilizing Cognos Analytics to its full potential for comprehensive data analysis. These skills are vital for professionals in data analysis, business intelligence, and decision-making roles, as they allow for more nuanced and insightful analysis of data. The ability to create interactive and detailed dashboards enhances one's capability to present data in a more engaging and informative manner. This knowledge is particularly beneficial for those seeking to improve their data presentation skills, making complex data more accessible and actionable for decision-makers. Overall, the lab provides a strong foundation in advanced data visualization techniques, making it a valuable learning experience for advancing one’s career in the field of data analytics. 

### Software

Like the videos in the course, for the hands-on labs, we will be using IBM Cognos Analytics trial version (currently limited to 30 days), as this is available at no charge.

### Dataset

The dataset used in this lab comes from the VM designed to showcase IBM Cognos Analytics. This dataset is published by IBM. You can download the dataset file directly from here: [CustomerLoyaltyProgram.csv](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DV0130EN-SkillsNetwork/Hands-on%20Labs/Lab%206%20-%20%20Advanced%20Dashboard%20Capabilities%20in%20Cognos%20Analytics/CustomerLoyaltyProgram.csv)

### Objectives

After completing this lab, you will be able to:

- Start a new dashboard
- Create calculations
- Keep/exclude data points from a visualization
- Set top/bottom on a visualization
- Create and leverage navigation paths
- Filter data in a dashboard

## Exercise 1: Start a New Dashboard

In this exercise, you will start a new dashboard for working with advanced Cognos Analytics dashboard capabilities.

**Step 1:** To sign in to the Cognos Analytics platform with your IBMid, go to [myibm.ibm.com/dashboard/](https://myibm.ibm.com/dashboard/?utm_source=skills_network&utm_content=in_lab_content_link&utm_id=Lab-IBMSkillsNetwork-DV0130EN-Coursera).

**Step 2:** Enter your IBMid and password.

**Step 3:** Scroll down and click **Launch**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/launch.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 4:** From the **Recent** section, click the uploaded data file **CustomerLoyaltyProgram.csv**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/3.B.1.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 5:** The template window will be displayed, allowing you to select the type of dashboard and the template style. Select the **Tabbed** dashboard style. This will allow you to have multiple pages for your dashboards. Select the *five-panel template*, then click **Create**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_1.5.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 6:** To save the newly created dashboard, press **CTRL+S** or click the **Save** icon and then click **Save as**. 

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_1.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div> 

**Step 7:** A new **Save as** window will pop up. Follow the steps as displayed below to save your dashboard as **Advanced Dashboard** in the **My content** section.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 8:** As you build the dashboard, the location placement for visualization widgets in the dashboard template will be referenced using the following Panel numbers.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_1.7.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 9:** From the **Navigation** panel, select **Sources** to ensure the data source panel is open in the left pane.

**Step 10:** From the data source panel, select **Revenue** and drag it to the center of **Panel 1**, releasing it once you see the drop zone turn blue.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_5.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 11:** Click the summary chart in Panel 1 to bring it into focus. From the on-demand toolbar that appears in the main toolbar, click **Summarize**, and then select **Average**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_6.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 12:** In the summary chart in Panel 1, select the title of the visualization and change it to *Average Revenue*.

**Step 13:** From the **Navigation** panel, select **Widgets** to open the widgets panel. Drag and drop **Money coin** from **Shapes** to the center of Panel 1.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_7.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 14:** To save the current work in the dashboard, press **CTRL+S** or click **Save** in the toolbar.

**Step 15:** Your Panel 1 visualization should look similar to the one below:

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_1.13.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

## Exercise 2: Working with Advanced Cognos Analytics dashboard capabilities

In this exercise, you will practice some advanced Cognos Analytics dashboard capabilities.
- Task A: Create calculations 
- Task B: Keep/Exclude Data Points from a visualization
- Task C: Set Top/Bottom on a visualization
- Task D: Create and Leverage navigation paths
- Task E: Filter Data in the current tab

### Task A: Create Calculations 

**Step 1:** From the **Navigation** panel, select **Sources** to open the data source panel if it is not already open. The data source panel displays the uploaded file **CustomerLoyaltyProgram.csv** as the selected source.

**Step 2:** Right-click the **CustomerLoyaltyProgram.csv** data source and select **Calculation**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2.A.2.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 3:** Change the calculation name to **Margin**. From the **Components** panel, drag **Unit Sale Price** to the **Expression** field, type a space, then the minus sign, **-**, to the right of it, and then drag **Unit Cost** to the right of that. Click **OK**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_8.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2.A.3.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 4:** In the data source panel, expand CustomerLoyaltyProgram.csv if needed, and drag **Margin** to the center of **Panel 2**, releasing it once you see the drop zone turn blue.

**Step 5:** Right-click the margin chart in Panel 2, point to **Summarize**, and then select **Average**.

**Step 6:** From the data source panel, right-click on **Margin** and click **Format data**. 

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_9.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 7:** In the **Format type** list, select **Currency**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_10.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 8:** Select **$ (USD) - United States of America, dollar** as the currency and click **OK** at the bottom.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_11.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 9:** In the margin chart in Panel 2, select the title of the visualization and change it to *Average Margin*.

**Step 10:** To save the current work in the dashboard, press **CTRL+S** or click **Save** in the main toolbar.

**Step 11:** Your Panel 2 visualization should look similar to the one below:

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2.A.9.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

### Task B: Keep/Exclude Data Points from a Visualization

**Step 1:** In the data source panel, expand CustomerLoyaltyProgram.csv if needed. Press the **CTRL** key and select **Revenue** and **Product Line** and drag them both to the center of **Panel 3**, releasing them once you see the drop zone turn blue.

**Step 2:** From the data source panel, drag **Location Code** to the **Color** drop zone of **Panel 3**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2.B.2.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 3:** Right-click the **Suburban** data point in the Panel 3 visualization, and select **Exclude**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2.B.3.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 4:** To save the current work in the dashboard, press **CTRL+S** or click **Save** in the main toolbar.

**Step 5:** Your Panel 3 visualization should look similar to the one below:

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2.B.5.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

### Task C: Set Top/Bottom on a Visualization

**Step 1:** From the data source panel, press the **CTRL** key and select **Quantity Sold** and **City**, and drag them both to the center of **Panel 4**, releasing them once you see the drop zone turn blue.

**Step 2:** Click the chart in Panel 4 to bring it into focus and render the on-demand toolbar.

**Step 3:** Click the **Change visualization** button in the on-demand toolbar (which will currently say **Map**), then expand **All visualizations**, if needed, and select **Column**.

**Step 4:** In Panel 4, right-click the axis label **Quantity Sold (Sum)** down the left side of the chart and select **Top or bottom**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2.C.4.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 5:** Ensure the value of **Number of results** is set to **10**, then select **Top count**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2.C.5.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 6:** In the column chart in Panel 4, select the title of the visualization and change it to *Top 10 Quantity Sold by City*.

**Step 7:** To save the current work in the dashboard, press **CTRL+S** or click **Save** in the main toolbar.

**Step 8:** Your Panel 4 visualization should look similar to the one below:

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2.C.8.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

### Task D: Create and leverage navigation paths

**Step 1:** In the data source panel on the left, scroll to the top of the list and click the **plus sign** labeled **Create navigation path** to the right of **Navigation paths**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2.D.1.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 2:** In the **Create navigation path** dialog box, expand CustomerLoyaltyProgram.csv, if needed. Drag **Order Year**, **Quarter**, **Country**, and **City** sequentially to the right hand panel of the dialog box, maintaining the order (shown in the image below). Once done, click **OK**. 

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2.D.2.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 3:** From the data source panel, press the **CTRL** key and select **Margin**, **Product Line**, and **Order Year** and drag them to the center of **Panel 5**, releasing them once you see the drop zone turn blue.

**Step 4:** Click the line chart in Panel 5 to bring it into focus and render the on-demand toolbar.

**Step 5:** Click the **Change visualization** button in the on-demand toolbar (which will currently say **Line**), then expand **All visualizations**, if needed, and select **Bar**.

**Step 6:** In Panel 5, right-click the axis label **Order Year** down the left side of the chart, and select **Navigate**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2.D.6.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 7:** One by one, select the **Order Year**, **Quarter**, **Country**, and **City** options in the **Navigate** dialog box to view the different navigation paths and observe the resulting visualization in Panel 5 as you select each one. Lastly, keep the **Order Year** option selected.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2.D.7.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 8:** <ins>Alternative interactive way with Drill down/back:</ins>
- In the bar chart in Panel 5, right-click the **2016** - **Smart Electronics** bar of the bar chart, and select **Drill down**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2.D.8.1.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

- Now right-click the **Q1** - **Smart Electronics** bar of the bar chart, and select **Back**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2.D.8.2.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 9:** To save the current work in the dashboard, press **CTRL+S** or click **Save** in the main toolbar.

**Step 10:** Your Panel 5 visualization should look similar to the one below:

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2.D.10.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

### Task E: Filter Data in the Current Tab

**Step 1:** If required, click **Filters** in the **Dashboard Toolbar** to display the filters pane.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2.E.1.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 2:** From the data source panel, select **Product Line** and drag it to the **This tab** filter panel on the right hand side.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2.E.2.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

**Step 3:** Click the **Product Line** filter tab of the **This tab** filter panel. Select **Computers and Home Office**, **Photography**, and **TV and Video Gaming**, then click **Done**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2.E.3.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

Your final dashboard should look similar to the one below. To save the current work in the dashboard, press **CTRL+S** or click **Save** in the main toolbar. 

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L3_2_final_dashboard.png" style="width:880px; max-height:500px; object-fit:contain;"></div></div>

Feel free to change the appearance and layout of the dashboard you have just created. 

**Congratulations!**

You have completed this lab!



