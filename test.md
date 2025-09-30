---
layout: page
title: Milanfx Study Notes
permalink: /xxx/
---



# Cognos Different Methods for Creating Dashboard

**Estimated Time Needed: 45 Minutes**

### Purpose of the Lab: 

This lab is meticulously designed to enhance skills in utilizing IBM Cognos Analytics for creating sophisticated dashboard visualizations. The primary objectives include working with tabs, initiating new dashboards within these tabs, and mastering different methods for crafting dashboard visualizations. The lab guides users through automatic and manual techniques for visualization creation, as well as leveraging Cognos Analytics Assistant for this purpose. The focus is on practical application, enabling users to navigate through various features of Cognos Analytics, such as employing various visualization styles (like radial charts and packed bubble charts), and understanding how to effectively use data to create meaningful and interactive dashboards. 

### Benefits of Learning the Lab: 

Participating in this lab provides invaluable benefits, particularly for those aspiring to excel in data analytics and visualization.You will gain hands-on experience in using IBM Cognos Analytics, a leading tool in the business intelligence domain. The skills acquired include creating diverse types of visualizations, understanding the application of different visualization methods, and effectively presenting data in an interactive and engaging manner. This knowledge is crucial for professionals in data analytics, marketing, business intelligence, and other fields that rely heavily on data visualization for decision-making and presentation purposes. The lab offers a robust foundation for those aiming to build or enhance their expertise in using advanced business intelligence software, thereby increasing their proficiency and employability in the rapidly evolving field of data analytics. 

### Software used in this lab

Like the videos in the course, for the hands-on labs, we will be using IBM Cognos Analytics trial version (currently limited to 90 or 30 days), as this is available at no charge.

### Dataset used in this lab

The dataset used in this lab comes from the VM designed to showcase IBM Cognos Analytics. This dataset is published by IBM. You can download the dataset file directly from here: [CustomerLoyaltyProgram.csv](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DV0130EN-SkillsNetwork/Hands-on%20Labs/Lab%204%20-%20Getting%20Started%20with%20Cognos%20Analytics/CustomerLoyaltyProgram.csv)

### Objectives

After completing this lab, you will be able to:
- Work with tabs
- Start a new dashboard within tabs
- Use an automatic method to create a visualization
- Use Cognos Assistant to create a visualization
- Use a manual method to create a visualization

## Exercise 1: Work with tabs and start a new dashboard within tabs

In this exercise, you will learn how to work with tabs and start a new dashboard within tabs.

**Step 1:** To sign in to the Cognos Analytics platform with your IBMid, go to [myibm.ibm.com/dashboard/](https://myibm.ibm.com/dashboard/?utm_source=skills_network&utm_content=in_lab_content_link&utm_id=Lab-IBMSkillsNetwork-DV0130EN-Coursera).

**Step 2:** Enter your IBMid and password.

**Step 3:** Scroll down and click **Launch**.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/launch.png "Lab2_Cognos_Launch"" width="400"></div></div>

**Step 4:** From the **Recent** section, double-click **Simple dashboard** to open it.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L2_I1.PNG "Lab2_Cognos_recent"" width="400"></div></div>

**Step 5:** Ensure that **Edit** is turned on in the top left corner. Then click the **Add new tab** button to the right of the **A - Product Sales** tab.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L2_I2.png "Lab2_Cognos_Add_Tab"" width="600"></div></div>

**Step 6:** Select the **four-panel template with 2x2 configuration**. Click **Create**.
<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L2_I3.PNG "Lab2_Cognos_template"" width="600"></div></div>

**Step 7:** Click the tab named **Tab 1** and select **Edit the title**. Rename the tab to **B - Customer**.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L2_I4.png "Lab2_Cognos_rename"" width="600"></div></div>

## Exercise 2: Differentm methods for creating dashboard visualizations

In this exercise, you will learn different methods for creating dashboard visualizations.

- As you build the dashboard, the location placement for widgets in the dashboard template will be referenced using the following panel numbers

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/2.1.png "Lab2_Cognos_template1"" width="600"></div></div>

### Task A: Using an automatic method to create a visualization for panel 1

**Step 1:** From the **Navigation** panel, select **Sources** to open the data source panel if it is not already open. The data source panel displays the uploaded file **CustomerLoyaltyProgram.csv** as the selected source.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/3.C.2.New.png "Lab2_Cognos_3_C_2_new"" width="400"></div></div>

**Step 2:** From the data source panel, expand CustomerLoyaltyProgram.csv if needed.

**Step 3:** From the data source panel, press the **CTRL** key, select **Latitude**, **Longitude**, and **Quantity Sold** and drag them to the center of **Panel 1**, releasing them once you see the **drop zone turn blue**.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/2.A.3.png "Lab2_Cognos_2.A.3"" width="600"></div></div>

The map will look like the following:

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L2_I5.png "Lab2_Cognos_map"" width="600"></div></div>

**Step 4:** Click the map chart in Panel 1 to bring it into focus.

**Step 5:** To change the map style, open the **Properties** panel and expand **Chart** to see the various options of maps available.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L2_I6.png "Lab2_Cognos_properties"" width="600"></div></div>

**Step 6:** In the **Map base** list, select **Streets**.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/Streets.png "Lab2_Cognos_Streets"" width="400"></div></div>

**Step 7:** Open the **Fields** panel to view the data slots. From the data source panel on the left of the screen, drag and drop **Country**, **Province or State**, and **Revenue** into the **Locations**, **Locations**, and **Location color** data slots of the **Regions** section of the Fields panel respectively.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/2.A.5.1.png "Labs_Cognos_fields"" width="400"></div></div>

**Step 8:** Expand the **Latitude/longitude** section of the Fields panel.

**Step 9:** Ensure that **Quantity Sold** is in the **Point color** data slot of the **Latitude/longitude** section of the Fields panel.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/2.A.6.png "Labs_Cognos_fields_2"" width="400"></div></div>

**Step 10:** Click the **Fields** button to close the fields panel.

**Step 11:** Click the map chart widget in Panel 1 to bring it into focus if needed. Select the title of the visualization and change it to *Revenue and Quantity Sold by Location*.

**Step 12:** Click the **Properties** button in the top right corner to open the **Properties** panel and click the **General** tab. Expand **Appearance**, click **Border color** to open the color options for borders, and select a black border.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L2_I8.png "Lab2_Cognos_Border"" width="600"></div></div>

**Step 13:** To save the current work of the dashboard, press **CTRL+S** or click the **Save** icon in the toolbar.

**Step 14:** Ensure that the **Regions** section has the correct fields in the relevant data slots as per the image in step 7 above.

**Step 15:** Your Panel 1 visualization should look similar to the one below:

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/2.A.12.New.png "Lab2_Cognos_final_dashboard1"" width="600"></div></div>

You can also change the visualization color palette as below:

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L2_I9.png "Lab2_Cognos_visuals"" width="400"></div></div>

For instance, in the below image, we have selected a Magenta palette.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L2_20.png "LAb2_Cognos_visuals_1"" width="600"></div></div>

### Task B: Using an automatic method to create a visualization for panel 2

**Step 1:** From the **Navigation** panel, click **Visualizations** and then select **Radial** chart from the visualizations.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L2_21.png "Lab2_Cognos_Radial"" width="600"></div></div>

**Step 2:** Click the **Fields** button on the dashboard toolbar to open the **Fields** panel.

**Step 3:** Drag and drop **Product Line** to the **Repeat (column)** data slot.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/2.B.5.png "Lab2_Cognos_Fields_3"" width="400"></div></div>

**Step 4:** Next, drag **Coupon Response** to the **Color** data slot. Also, drag **Coupon Response** to the **Bars** data slot, and then drag **Quantity Sold** to the **Length** data slot. 

**Step 5:** Click the **Fields** button to close the Fields panel. 

**Step 6:** Click the radial chart widget in Panel 2 to bring it into focus if needed. Select the title of the visualization and change it to *Product Line by Product Line and Coupon Response colored by Coupon Response*.

**Step 7:** Click the **Properties** button in the top right corner to open the **Properties** panel and click the **General** tab. Expand **Appearance**, click **Border color** to open the color options for borders, and select a black border.

**Step 8:** To save the current work of the dashboard, press **CTRL+S** or click the **Save** icon in the toolbar.

**Step 9:** Your Panel 2 visualization should look similar to the one below:

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/panel2.png "Dashboard_panel2"" width="600"></div></div>

### Task C: Using Cognos Assistant to create a visualization for panel 3

**Step 1:** From the Cognos Analytics main toolbar at the top right of the screen, click the **Assistant** icon to open the **Cognos Assistant** panel.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L2_23.png "Lab2_Cognos_assistant"" width="600"></div></div>

**Step 2:** In the **Ask a question** input text box, at the bottom of the right hand pane, type *show Quantity Sold and City* and press **Enter** or click the **Ask question** arrow.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L2_24.png "Lab2_Cognos_assistant1"" width="400"></div></div>

It will show you visualizations created automatically based on your question as below: 

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/L2_251.png "Lab2_Cognos_assistant2"" width="600"></div></div>

**Step 3:** Scroll down the pane and click **Show related visualizations**.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DV0130EN-SkillsNetwork/Hands-on%20Labs/Lab%205%20-%20Different%20Methods%20for%20Creating%20Dashboard%20Visualizations%20with%20Cognos%20Analytics/images/2.C.4.New.png" width="400"></div></div>

**Step 4:** Select the second chart visualization.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/Assistant_1.png "Lab2_Cognos_Assistant_1"" width="400"></div></div>

**Step 5:** From the **Cognos Assistant** panel, select the second chart visualization and drag it to the center of **Panel 3**, releasing it once you see the **drop zone turn blue**.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/Assistant_2.png "Lab2_Cognos_Assistant_2"" width="600"></div></div>

**Step 6:** Click the **Quantity Sold and Unit Cost by City** chart in **Panel 3** to bring it into focus if needed.

**Step 7:** Open the **Properties** panel and click the **General** tab. Expand **Appearance**, click **Border color** to open the color options for borders, and select a black border.

**Step 8:** To save the current work of the dashboard, press **CTRL+S** or click the **Save** icon in the toolbar.

**Step 9:** Your Panel 3 visualization should look similar to the one below:

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/Assistant_3.png "Lab2_Cognos_Assistant_3"" width="600"></div></div>

### Task D: Using a manual method to create a visualization for panel 4

**Step 1:** From the **Navigation** panel, select **Visualizations** to open the visualizations library.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DV0130EN-SkillsNetwork/Hands-on%20Labs/Lab%205%20-%20Different%20Methods%20for%20Creating%20Dashboard%20Visualizations%20with%20Cognos%20Analytics/images/2.D.1.New.png" width="400"></div></div>

**Step 2:** Select the **Packed Bubble** chart from the list.

**Step 3:** The packed bubble chart visualization will be added to Panel 4 of the dashboard template, and its **Fields** panel will be open, ready for you to set up the data definitions for your visualization.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DV0130EN-SkillsNetwork/Hands-on%20Labs/Lab%205%20-%20Different%20Methods%20for%20Creating%20Dashboard%20Visualizations%20with%20Cognos%20Analytics/images/2.D.2.New.png" width="600"></div></div>

**Step 4:** From the data source panel on the left of the screen, drag and drop the **Product Line**, **Quantity Sold**, and **Loyalty Status** sources into the **Bubbles**, **Size**, and **Color** data slots of the Fields panel respectively.

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DV0130EN-SkillsNetwork/Hands-on%20Labs/Lab%205%20-%20Different%20Methods%20for%20Creating%20Dashboard%20Visualizations%20with%20Cognos%20Analytics/images/2.D.3.New.png" width="600"></div></div>

**Step 5:** Click the **Fields** button to close the panel.

**Step 6:** Click the packed bubble chart visualization in Panel 4 to bring it into focus. Select the title of the visualization and change it to *Department Sales by Loyalty Status*.

**Step 7:** Open the **Properties** panel and click on the **General** tab. Expand **Appearance**, click **Border color** to open the color options for borders, and select a black border.

**Step 8:** To save the current work of the dashboard, press **CTRL+S** or click the **Save** icon in the toolbar.

**Step 9:** Your Panel 4 visualization should look similar to the one below:

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/Assistant_4.png "Lab2_Cognos_Assistant_4"" width="600"></div></div>

Finally, your dashboard **B - Customer** should look similar to the one below:

<div align="center"><div style="display: inline-grid; border: 3px solid DarkGreen;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DV0130EN-Coursera/images/B_customer_dashboard.png "Lab2_Cognos_B_Customer_Dashboard"" width="600"></div></div>

**Congratulations!**

You have completed this lab, and you are ready for the next topic.





