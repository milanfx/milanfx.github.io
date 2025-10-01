---
layout: page
permalink: /BI03Lab09/
---

# Lab09 - Looker Advanced Dashboard

**Estimated Time Needed: 60 Minutes**

### Purpose of the lab:

This hands-on lab focuses on enhancing skills in utilizing advanced features of Google Looker Studio to create dynamic and interactive dashboards. It covers creating calculated fields, manipulating data points within visualizations, applying filters, and constructing navigation paths. This lab provides hands-on experience aimed at leveraging Google Looker Studio for complex data analysis and visualization tasks.

### Software

Google Looker Studio, available for free.

### Dataset

Use data set [CustomerLoyaltyProgram.csv](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/bXn-QnrBL0Uv_nAaMVWgpw/CustomerLoyaltyProgram%20.csv "CustomerLoyaltyProgram.csv").

### Objectives:

- Start a new dashboard
- Use advanced Google Looker Studio dashboard capabilities
- Create a bar chart using Drill Down 
- Create another bar chart to implement top/bottom filtering in visualizations
- Create a horizontal bar chart using Drill Down and a calculated field
- Create a pie chart
- Add headings to all the created charts in the dashboard
- Build an interactive dashboard
- Save the dashboard and download as a PDF

## Step-by-step instructions

**Step 1:** **Starting a new dashboard**

a. Sign in to Google Looker Studio:

- Go to Google Looker Studio and sign in with your Google account.

b. Access the data set

- Here you are going to use the same data set that you have used in the previous lab and follow the same steps to upload the file.
- In the top left corner, click **Create**, then select **Data source**.
- In the **Search** box, type *file upload*, then click the **File Upload** connector.
- Click the **CLICK TO UPLOAD FILES** button, select the **CustomerLoyaltyProgram.csv** file, and click **Open**.
- Once the data is uploaded, click **CONNECT**.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/mzGSXG9vyEALK3SxzgjDkg/Advanced-Lab-Fig%200.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

c. Create and add the report

- To start creating the report, click **CREATE REPORT**.
- In the pop-up dialog box, click **ADD TO REPORT**.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/Z7xNUKltE7vl9_sybXJ5gw/Advanced-Lab-Fig%201.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

d. Save the new report

- Click the untitled report at the top and rename it to *Advanced Dashboard*.
- Save the new report.

**Step 2:** **Working with advanced Google Looker Studio dashboard capabilities**

a. Create calculations

- In your Data Source, click **+ ADD A FIELD**.
- Then select **Add calculated field**.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/gRkVFXJKzT7LrZ01QK34Wg/Advanced-Lab-Fig%202.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

- Define the calculation for Margin as **Unit Sale Price - Unit Cost**.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/mUGB-J0MGqf_hlMtPSRGgQ/Advanced-Lab-Fig%203.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

- Name the field **Margin** and save it.

b. Set up filters and control widgets
- Add filter controls.
- From the toolbar, select **Add a control** and choose a drop-down list or slider based on the type of filter you need, such as **City**.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/thrVidrnI93XYxo5ctg8cw/Advanced-Lab-Fig%204.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

- Position the filter control on the dashboard.

c. Add score cards

- Now you will include two scorecards to display *Margin* and *Revenue* on the top of your dashboard.
- In the toolbar, click **Add a chart**, and select **Scorecard**.
- Move it above the line chart visualization and to the left side of the canvas.
- And pick **Margin** to be displayed on this scorecard.
- In the Chart – Set Up area, click the left side of the **Margin** field and then you will see the following dialog box.  
- Select the data type and aggregation.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/BerexUOejqyb2CZeNiFubg/Advanced-Lab-Fig%204A.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

- You can change the size and position as you like.
- Use the **STYLE** tab in the scorecard chart\'s **Properties** pane to change the color and change the font size to **28pt** and then select **Background and Border**.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/peE0c-wQgVmCtK7U-Pp7MA/Advanced-Lab-Fig%204B.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

- Now you will add the second scorecard chart above the line chart.
- In the toolbar, click **Add a chart**, and select **Scorecard**.
- Place it to the right of the **Revenue** scorecard chart.
- Select the data type and aggregation.
- Then use the same size and style as **Margin**.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/nf9fKqm0hPha_vf6Rm2x8Q/Advanced-Lab-Fig%205.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

**Step 3:** **Creating a bar chart**

a. Create a bar chart (Revenue By Product Line By Location Code) using Drill Down

- Add a bar chart to your dashboard.
- Then drag the **Product Line** field to **Dimensions** (in the SET UP area)
- Then drag the **Location Code** field to **Breakdown Dimension**
- Then drag the **Revenue** field to **Metric** (change it to Average)

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/ljFH7Xvn_Ev4rCbohEhbVQ/Advanced-Lab-Fig%206.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

b. Exclude data points from the visualization

- Add a filter in the **Location Code**

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/7sdRuSMD2cmd6DrUX_3Mzg/Advanced-Lab-Fig%207.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

- And exclude **Suburban**

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/mapxLLZs5lvkUrbaxsvVbw/Advanced-Lab-Fig%208.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

**Step 4:** **Creating another bar chart to implement top/bottom filtering in visualizations**

- Add a bar chart to your dashboard.
- Sort the data in the chart\'s data properties
- Limit the number of bars to show top 10
- Then drag the **City** field to **Dimensions** (in the SET UP area)
- Then drag the **Quantity Sold** field to **Metric**

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/WCB2GmkdF2ToD3-_IJll3g/Advanced-Lab-Fig%209.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

**Step 5:** **Creating a horizontal bar chart (Margin By Order Year Colored By Product Line) using Drill Down**
- Add a horizontal bar chart to your dashboard
- Then drag the **Order Year** field to **Dimensions** (in SET UP area)
- Then drag the **Product Line** field to **Breakdown Dimension**
- Then drag the **Margin** calculated field to **Metric**

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/lJb8hwLfDH3lflk1EEuChg/Advanced-Lab-Fig%2010.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

**Step 6:** **Creating a pie chart of Loyalty Status Distribution**

- Add a pie chart to your dashboard
- Then drag the **Loyalty Status** field to **Dimensions** (in the SET UP area)
- Then drag the **Loyalty#** field to **Metric**

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/rCEFhlPo9kfqTHix6ibCfw/Advanced-Lab-Fig%2011.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

**Step 7:** **Adding headings to all the created charts in the dashboard**

- On the top of each chart, add a text box and enter the heading and use the text properties to make the text bold and fill it with color and provide a boundary.

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/At88omr4SwspDnKlvjW6RA/Advanced-Lab-Fig%2011A.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

**Step 8:** **Building an interactive dashboard**

- Filter data in the current tab (selecting a city)

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/DyKDdY9sgJZlcITeyIRdLA/Advanced-Lab-Fig%2012.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

- Filter data in the current tab (selecting a product line)

<div align="center"><div style="display: inline-grid; border: 2px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/Gt8RMPajm1HLD2inOJdN8g/Advanced-Lab-Fig%2013.png" style="width:890px; max-height:600px; object-fit:contain;"></div></div>

**Step 9:** **Saving the dashboard and downloading as a PDF**

- Finalize the dashboard.
- Ensure all visualizations are correctly configured and aligned.
- Preview the dashboard in **View** mode to check interactivity and finalize the design.
- Save the dashboard.
- Download as a PDF (you can also share your PDF).

**Congratulations!**

You have completed this lab!
