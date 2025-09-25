---
layout: page
title: Milanfx Study Notes
permalink: /xxx/
---


## Lab: Load data into the IBM Db2 database from a CSV file

### **Lab Overview:**

Now that you have learned about the process of importing data into a data repository from varied sources, you will load data from a CSV file into the IBM Db2 database instance you created in the previous lab.

**Estimated time needed:** 15 minutes

### **Dataset used in this exercise:**

The dataset used in this exercise comes from the following source: [https://www.kaggle.com/antfarol/car-sale-advertisements](https://www.kaggle.com/antfarol/car-sale-advertisements) under a [CC0: Public Domain license](https://creativecommons.org/publicdomain/zero/1.0/). We are using a modified subset of that dataset for this lab. To follow the lab instructions successfully, please use the dataset provided with this exercise rather than the dataset from the original source.

**NOTE:** The lab assumes that you have downloaded this CSV file: [exercise03_car_sales_data.csv](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/exercise03_car_sales_data.csv) to your local system.

Please follow the steps given below to provision your instance of IBM Db2 on Cloud.

**Step1:** Go to: [https://cloud.ibm.com/catalog/services/db2](https://cloud.ibm.com/catalog/services/db2?utm_source=skills_network&utm_content=in_lab_content_link&utm_id=Lab-IBM-DB0100EN-SkillsNetwork) to access your Db2 dashboard on Cloud.

**Step2:** If you’re not already logged in to your IBM Cloud Lite account, click on **Log in** at the bottom right of the screen to log in.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-1.png" width="400"></div>

**Step3:** Logging in will take you to your **Db2 service dashboard**.

Click on **view existing** link in the **Existing Lite plan instance** box.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-2.png" width="400"></div> 

**Step4:** The **Manage** tab will be active by default in your services dashboard. Click on **Go to UI**.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-3.png" width="800"></div> 

**Step5:** Now click on the menu bar icon in the top left corner of your Db2 service dashboard.

Click on **Load** **>** **Load Data**.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-4.png" width="800"></div> 

**Step6:** You can either drag and drop the CSV file into the **File selection** box, or you can click on the **browse files** link, also provided in the **File selection** box to browse your local folders to find and open the downloaded CSV file.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-5.png" width="800"></div> 

The name of the CSV file you have uploaded will appear in the **Selected file** section on the right.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-6.png" width="800"></div> 

Click **Next** to proceed.

**Step7:** You will be asked to select a **Schema** from a list of schema names.

**NOTE:** Select the schema name with a random mix of alphabets and numbers. It will be similar to, but not the same as, the one you see in the screenshot below (_MGJ73335_). The ones that you do NOT have to select are AUDIT, DB2INST1, ERRORSCHEMA, and ST_INFORMTN_SCHEMA (and sometimes you might also see SQLxxxxx as well).

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-7.png" width="800"></div>

**Step8:** Click on **New Table**.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-8.png" width="800"></div> 

**Step9:** Enter the name **CARSALESTABLE** in the input box prompting you with **_NEW TABLE NAME_**.

**Note:** You will be using this table name in the SQL queries you will execute in the next exercise.

Now click on **Create** to create the new table.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-9.png" width="800"></div> 

**Step10:** A table by the name of **CARSALESTABLE** has been created.

Click **Next** at the bottom right of the page to proceed.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-10.png" width="800"></div> 

**Step11:** Click **Next** to proceed.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-11.png" width="800"></div>

**Step12:** Then click **Begin Load** to begin the process of loading the data from the CSV into your database.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-12.png" width="800"></div> 

**Step13:** Data from your CSV file is now loaded into your Db2 instance.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0100EN-SkillsNetwork/labs/images/Figure_3-13.png" width="800"></div> 

Congratulations! You have successfully loaded data from a CSV file into the IBM Db2 instance you created in the previous lab.


---

## Create an IBM Cloud Account

1. Once you are on the [account creation](https://cloud.ibm.com/registration?utm_source=skills_network&utm_content=in_lab_content_link&utm_id=Lab-IBM-CC0100EN-SkillsNetwork) page, follow the below instructions to create an IBM cloud trial account.

2. Enter your **Email** address [preferably use Gmail ID or Yahoo ID] and a strong **Password**, as per criteria, and then click the **Next** button.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CC0100EN-SkillsNetwork/images/IBM_signup.png" width="800"></div>

> **NOTE:** Please ensure that you provide an email address that you have not used previously to create any other IBM Cloud account, and you can readily access your email to retrieve the verification code required in the next step.

3. An email is sent to the address you signed up with to confirm your email address. Check your email and copy and paste **Verification code**. Then click **Next**.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CC0100EN-SkillsNetwork/labs/IBMCloud_accountCreation/images/Step_3.png" width="800"></div>

4. Once your email is successfully verified, enter your **First name** and **Last name**, and select your country (for example, United States) under **Country or region** then click **Next**.

>**Note:** Kindly use your full last name instead of just using single letters/initials. For example:
First Name: Ada
Last Name: Lovelace

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CC0100EN-SkillsNetwork/labs/IBMCloud_accountCreation/images/Step_4.png" width="800"></div>

5. Go through the Account Notice. If you wish, you can opt for email updates. Then accept the Terms and Conditions and click **Continue**.  

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CC0100EN-SkillsNetwork/labs/IBMCloud_accountCreation/images/Step_5.png" width="800"></div>

6. Before creating your account, review the account privacy notice and acknowledge that you have read and understood by checking the checkbox and clicking **Continue**.  

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CC0100EN-SkillsNetwork/labs/IBMCloud_accountCreation/images/Step_6.png" width="800"></div>

> It takes a few seconds to create and set up your account.

7. On the next screen, you will be asked to verify your identity where you will see the feature code has been applied for you already. Then click on **Create account**. 

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CC0100EN-SkillsNetwork/labs/IBMCloud_accountCreation/images/verify_identity.png" width="800"></div>

> **Note:** It might take a couple of minutes to create your account.

> **Note:** Please ensure you do not use the Credit Card option to verify your account for coursework as that can result in unnecessary charges and delays in activating your account.

8. Once you have successfully created your IBM Cloud account, you should see the dashboard.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CC0100EN-SkillsNetwork/images/IBM-dashboard.png" width="800"></div>

9. Now you may explore the [IBM Catalog](https://cloud.ibm.com/catalog?utm_source=skills_network&utm_content=in_lab_content_link&utm_id=Lab-IBM-CC0100EN-SkillsNetwork) for exploring the services and resources offered by IBM Cloud.

<div align="center"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-CC0100EN-SkillsNetwork/labs/IBMCloud_accountCreation/images/catalog.png" width="800"></div>

---

## Ways To Troubleshoot

If you encounter any of the below errors while activating your IBM Cloud trial account, please follow the steps as instructed below.

- Ooops snap! The promotional codes for IBM Cloud are very popular and have temporarily run out. Please check back soon.

    **Reason** - It takes 24 to 48 hours to populate news feature codes.

    **Solution** - Please try again later

- Something went wrong error.

    **Reason** - This could be because you have already applied a code to this email earlier or your domain/country/IP is restricted.

    **Solution** - Try from another email id

- Feature code expired.

    **Reason** - You may have applied the feature code already once.

    **Solution** - Create a new IBM cloud account and write to the support team as per the instructions below.

- If your trial ends.

    **Reason** - Trial accounts are valid only for 6 months, and the same feature code cannot be applied again.

    **Solution** - Create a new IBM cloud account and write to the support team as per the instructions below.

---

## Other Possible Solutions:

- Try clearing your browser\'s cache and cookies
- Try from a different browser on an incognito mode.

If you still face any issues, please write an email to support@cognitiveclass.ai with the following details

**Subject Line:** Feature Code Issue

**Email Content:**

- Name of the course you are undertaking.
- The course link where you obtained the feature code.
- The feature code you are trying to apply.
- The error message that it is shown.
- The email ID used to create the IBM Cloud account.
- Your username.

Once you obtain a new feature code, you can create a new account using a different Email ID.

Congratulations! You have successfully created your IBM Cloud Account!


---

## Practice exercise

Create a script named `greetnew.sh` that takes the first and last names of the user, saves them in corresponding variables `firstname` and `lastname`, and prints a welcome message, such as `"Hello <firstname> <lastname>"`.

Use the `read` command and `echo` commands. Write comments. Make sure to add the shebang line.

Step 1: Create a new file named `greetnew.sh`.

Step 2: Add the following lines to the file:

<pre><code>
      #! /bin/bash
      
      # This script accepts the user's name and prints 
      # a message greeting the user
      
      echo -n "Enter your firstname :"	  	
</code></pre>

Step 3: Save the file.

Step 4: Add the execute permission to `greetnew.sh` for the owner:

```
chmod u+x greetnew.sh
```

Step 5: Execute the file from the command prompt using the following command:

```
./greetnew.sh
```

### Summary

In this lab, you learned how to:
- Create and execute a simple Bash shell script
- Implement the shebang directive `#! /bin/bash` in a Bash shell script
