---
layout: page
title: Milanfx Study Notes
permalink: /xxx/
---


# Cloudant Practice

**Estimated Time Needed: 45 Minutes**

### Overview

You\'ll now put into practice the skills you learnt working with Cloudant.

### Objectives

- Export data from a Cloudant database
- Import data into a Cloudant database
- Replicate a Cloudant database
- Create indexes on a Cloudant database
- Query data in a Cloudant database

### About This SN Labs Cloud IDE

This Skills Network Labs Cloud IDE provides a hands-on environment for course and project-related labs. It utilizes Theia, an open-source IDE (Integrated Development Environment) platform that can be run on a desktop or the cloud. To complete this lab, you will also need an instance of Cloudant running in IBM Cloud.

### Important notice about this lab environment

Please be aware that sessions for this lab environment are not persisted. Every time you connect to this lab, a new environment is created for you. Any data you may have saved in the earlier session would get lost. Plan to complete these labs in a single session to avoid losing your data.

### Working with Files in Cloud IDE

If you are new to Cloud IDE, this section will show you how to create and edit files that are part of your project in Cloud IDE.

To view your files and directories inside Cloud IDE, click the file icon to reveal it.

![Files icon highlighted to reveal project directory](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/empty-project-directory-icon-selected.png "Files icon highlighted to reveal project directory")

If you have cloned (using the `git clone` command) boilerplate/starting code, then it will look like the image below:

![Project directory showing boilerplate code](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/boilerplate-code.png "Project directory showing boilerplate code")

If you have not cloned and are starting with a blank project, it will look like this:

![Empty project directory](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/empty-project-directory.png "Empty project directory")

### Create a New File

To create a new file in your project, right-click and select the New File option.  You can also choose `File -> New File` to do the same.

![Create new file menu](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/create-new-file-menu.png "Create new file menu")


You will then be prompted to name the new file. In this scenario, let\'s name it  `sample.html`.

![New file name](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/new-file-name.png "New file name")

Clicking the file name `sample.html` in the directory structure will open the file on the right pane. You can create all different types of files. For example, `FILE_NAME.js` for JavaScript files.

![Viewing sample file](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/viewing-sample-file.png "Viewing sample file")

In the example below, we pasted some basic HTML code and then saved the file.

![Editing sample file](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/editing-sample-file.png "Editing sample file")

We save this file by:
- Going in the menu
- Press `Command + S` on Mac or `CTRL + S` on Windows
- Alternatively, it will Autosave your work as well

![Save file menu](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/save-file.png "Save file menu")


## Set-up: Create IBM Cloud Account

To access the resources and services that the IBM Cloud provides, you need an IBM Cloud Account. This lab will take you through step-by-step instructions to create IBM Cloud Account.

### Activate Trial Account

1. The previous section of the lab is the first step for activating your IBM Cloud trial account using Feature Code.

2. On clicking on `Open Tool` button, you will get a unique code.

3. Next, click on Activate Your Trial. It will redirect you to the IBM Cloud registration page, to create an account on IBM Cloud.

![activate trial account](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/activate_trial_account.png "activate trial account")

### Create an IBM Cloud Account

1. Once you are on the [account creation](https://cloud.ibm.com/registration?utm_source=skills_network&utm_content=in_lab_content_link&utm_id=Lab-IBMSkillsNetwork-DB0151EN-edX) page, follow the below instructions to create an IBM cloud trial account.

2. Enter your **Email** address [preferably use Gmail ID or Yahoo ID] and a strong **Password**, as per criteria and then click the **Next** button.

![enter email address and password](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/enter_details.png "enter email address and password")

**NOTE:** Please ensure that you provide an email address that you have not used previously to create any other IBM Cloud account, and you are able to readily access your email to retrieve the verification code required in the next step.

3. An email is sent to the address that you signed up with to confirm your email address. Check your email and copy and paste **Verification code**. Then click **Next**.

![verify email](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/verify-email.png "verify email")

4. Once your email is successfully verified, enter your **First name**, **Last name**, and preferably select **United States** under **Country or region** then click **Next**.

**Note:** Kindly use your full last name instead of just using single letter/initials.

Example: 

First Name: test

Last Name: skillup

![personal information](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/personal-information.png "personal information")

5. Go through the Account Notice and opt for Email updates if you desire, accept the terms and conditions and click on **Continue**.

![accept and continue](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/accept-and-continue.png "accept and continue")

6. Before creating your account, review the account privacy notice and acknowledge that you have read and understood by checking the checkbox and click on Continue

![accept privacy notice](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/accept-privacy-notice.png "accept privacy notice")

It takes a few seconds to create and set up your account.

7. On the next screen, you will be asked to verify identity where you will see the feature code has been applied for you already. Then click on **Create account**.

![verify identity](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/verify_identity.png "verify identity")

**Note:** It might take a couple of minutes to create your account.

**Note:** Please ensure you should not use the Credit Card option to verify your account for course work as that can result in unnecessary charges and delays in activating your account.

8. Once you have successfully created your IBM Cloud account, you should see the dashboard.

![ibm cloud dashboard](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/ibm-cloud-dashboard.png "ibm cloud dashboard")

9. Now you may explore the [IBM Catalog](https://cloud.ibm.com/catalog?utm_source=skills_network&utm_content=in_lab_content_link&utm_id=Lab-IBMSkillsNetwork-DB0151EN-edX) for exploring the services and resources offered by IBM Cloud.

![ibm cloud catalog](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/catalog.png "ibm cloud catalog")

## Set-up: Create IBM Cloudant Instance

### Create an IBM Cloudant instance

- Click on [cloud.ibm.com/catalog/services/cloudant](https://cloud.ibm.com/catalog/services/cloudant?utm_source=skills_network&utm_content=in_lab_content_link&utm_id=Lab-IBMSkillsNetwork-DB0151EN-edX) to create a Cloudant instance.

Or you can alternatively click on `Create Resource`, search for Cloudant on the Dashboard page.

You will be taken to the Cloudant instance creation page.

![cloudant create instance](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/cloudant-create-instance.png "cloudant create instance")

- Select the region under the \"Available regions.\"

It is OK to go with the default option, if you cannot figure out which region to choose.

- Scroll down to configure Cloudant instance.

![cloudant create instance steps](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/cloudant-create-instance-steps.png "cloudant create instance steps")

- Set your instance name to `mycloudant` or anything else that you prefer.

- Authentication Method is a critical setting. Select \"IAM and legacy Credentials\" as your Authentication Method. If you choose any other Authentication Method, some labs will not work.

- Select the **Lite** plan.

- Click on `Create`

You should see a screen like this:

![service created](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/cloudant-instance-create2.png "service created")

Your Cloudant service will be created and you will be redirected to the Resource list page.

- If you are not redirected, you can click on this link [cloud.ibm.com/resources?groups=resource-instance](https://cloud.ibm.com/resources?utm_source=skills_network&utm_content=in_lab_content_link&utm_id=Lab-IBMSkillsNetwork-DB0151EN-edX&groups=resource-instance)

You may see a screen like this, indicating the Provision in progress.

![resources list](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/cloudant-instance-create3.png "resources list")

- Wait till the status turns \'Active\' and click on `mycloudant` or your custom instance name.

![mycloudant resource created](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/cloudant-instance-create4.png "mycloudant resource created")

You will be taken to the Cloudant instance page.

You have successfully created the Cloudant instance.

### Create Cloudant Service credentials

- On the Cloudant instance page, click on `Service Credentials`

![cloudant instance page](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/cloudant-instance-page.png "cloudant instance page")

- Click on `New Credential`

![new credentials button](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/create-credentials1.png "new credentials button")

- Create credential pop up appears. Accept the default values for Name and Role and click on `Add`

![add credentials](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/create-credentials2.png "add credentials")

- Your Cloudant Service credentials will be created. Click on the chevron to view the credentials.

DO NOT attempt to use the credentials shown here. These are expired credentials.

![view credentials](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/create-credentials3.png "view credentials")

- You will be using the username, password and url in the next labs.

![credential details](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/create-credentials4.png "credential details")

![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/labs/Cloudant/images/create-credentials4.png)

You have successfully created a Cloudant instance and Service credentials for your instance.

Note: If you do not see the password field in your credentials, it is because in Exercise 2, Step 5 you have not selected \"IAM and legacy credentials.\" You can fix it by deleting your current Cloudant instance and following this lab from the beginning to create a new instance of Cloudant.

## Set-up: Using HTTP API to create and query Cloudant databases

Before you start working with the HTTP API to access the Cloudant, you need to collect the below details of your Cloudant instance, from the Service Credentials.

1. Your Cloudant username

2. Your Cloudant password

3. Your Cloudant URL

![credential details](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/create-credentials4.png "credential details")

Copy the `url` without the double quotes on either side.

Replace the value of `CLOUDANTURL` given below with yours.

DO NOT use the values given below. They are all expired credentials.

After replacing with your credentials, copy and paste the below command on the terminal.

This url contains your Cloudant username and password. DO NOT MAKE IT PUBLIC OR SHARE IT WITH ANYONE.

```bash
export CLOUDANTURL="<COPIED_VALUE>"
```

Test if you can reach your Cloudant server from the lab environment.

Run the below command on the terminal.

```bash
curl $CLOUDANTURL
```

If you get an output similiar to the one below, it means you are able to reach your Cloudant server.


![curl cloudant outcome](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/output2.png "curl cloudant outcome")

Test your credentials.

```
curl $CLOUDANTURL/_all_dbs

```

![all dbs outcome](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-DB0151EN-edX/images/output3.png "all dbs outcome")

If you get a list of your databases, it indicates that your credentials are correct. Now we can proceed with the rest.

## Exercise 1 - Cloudant export data

Before going ahead set the environment varible `CLOUDANTURL` to your actual cloudant url from your service credentials.

### Create sample data

Let\'s create some data if you don\'t have already.

```bash
curl -X DELETE $CLOUDANTURL/diamonds
curl -X PUT $CLOUDANTURL/diamonds

curl -X PUT $CLOUDANTURL/diamonds/1 -d '{
    "carat": 0.31,
    "cut": "Ideal",
    "color": "J",
    "clarity": "SI2",
    "depth": 62.2,
    "table": 54,
    "price": 339
  }'

curl -X PUT $CLOUDANTURL/diamonds/2 -d '{
    "carat": 0.2,
    "cut": "Premium",
    "color": "E",
    "clarity": "SI2",
    "depth": 60.2,
    "table": 62,
    "price": 351
  }'
```

### Export in CSV format

Export data from the `diamonds` database into csv format.

```
couchexport --url $CLOUDANTURL --db diamonds --delimiter ","
```

You should see all the documents in the `diamonds` database printed in csv format.

### Export in JSON format

Export data from the `diamonds` database into json format (one document per line).

```
couchexport --url $CLOUDANTURL --db diamonds --type jsonl
```

You should see all the documents in the `diamonds` database printed in json format.

Export data from the `diamonds` database into json format and save to a file named `diamonds.json`.

```
couchexport --url $CLOUDANTURL --db diamonds --type jsonl > diamonds.json
```

Export data from the `diamonds` database into csv format and save to a file named `diamonds.csv`.

```
couchexport --url $CLOUDANTURL --db diamonds --delimiter "," > diamonds.csv
```

## Exercise 2 - Import data into Cloudant

Right-click on the link and \"open in a new tab\" to obtain the content of the json file and copy the entire content: <a href="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0151EN-SkillsNetwork/labs/Final%20Assignment/data/movie.json" target="_blank">movies.json</a>

Now, go to the lab environment by clicking on the Launch/Open Tool button, and create a new file named movie.json under the project directory and paste the entire content copied earlier into the newly created json file.

### Import data from json into your Cloudant Database

Go to your Cloudant Service created on IBM Cloud and then click on Launch Dashboard to launch the cloudant databases. Then, click on New database on the top-right corner and create a Non-patitioned database named movies.

Run the given command in the terminal to import `movies.json` into your Cloudant database `movies`:

```bash
curl -XPOST $CLOUDANTURL/movies/_bulk_docs -Hcontent-type:application/json -d @movies.json
```

## Exercise 3 - Replicate a local database into your Cloudant instance

Using the replication page in the Cloudant dashboard, replicate the below source database using one time replication.

Source

- Type: Local Database

- Name: movies

- Authentication : IAM Authentication

Add your Cloudant API key below (you can find it in the service credentials tab).

Target

- Type: New local database

- Authentication : IAM Authentication

Add your Cloudant API key below (you can find it in the service credentials tab).

Options

- Replication type: One time

Click on Start Replication

## Exercise 4 - Create indexes using HTTP API

### Create an index for the \"Director"

<details>
<summary>Click here for Hint</summary>

use curl command with the POST and use the index key in the  JSON document.

</details>

<details>
<summary>Click here for Solution</summary>

```bash
curl -X POST $CLOUDANTURL/movies/_index \
-H"Content-Type: application/json" \
-d'{
    "index": {
        "fields": ["Director"]
    }
}'

```

</details>

### Create an index for the \"title"

<details>
<summary>Click here for Hint</summary>

use curl command with the POST and use the index key in the  JSON document.

</details>

<details>
<summary>Click here for Solution</summary>

```bash
curl -X POST $CLOUDANTURL/movies/_index \
-H"Content-Type: application/json" \
-d'{
    "index": {
        "fields": ["title"]
    }
}'

```

</details>

## Exercise 5 - Query data using HTTP API

### Find movies by Director

Write a query to find all movies directed by \'Richard Gage\' using the HTTP API

<details>
<summary>Click here for Hint</summary>

use curl command with the POST and include the field `Director` in the query JSON document.

</details>

<details>
<summary>Click here for Solution</summary>

```bash
curl -X POST $CLOUDANTURL/movies/_find \
-H"Content-Type: application/json" \
-d'{ "selector":
        {
            "Director":"Richard Gage"
        }
    }'

```

</details>

### Find movie by title

Write a query to list only the `year` and `Director` keys for the `title` \'Top Dog\' movies using the HTTP API.

<details>
<summary>Click here for Hint</summary>

use curl command with the POST and include the field `title` in the query JSON document.

</details>

<details>
<summary>Click here for Solution</summary>

```bash
curl -X POST $CLOUDANTURL/movies/_find \
-H"Content-Type: application/json" \
-d'{ "selector":
        {
            "title":"Top Dog"
        },
	"fields": ["year", "Director"]
    }'

```
</details>

### Summary

**Congratulations!**

In this lab, you have practiced the skills you learnt using IBM Cloudant.














