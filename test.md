---
layout: page
title: Milanfx Study Notes
permalink: /xxx/
---


# Download-Install-Anaconda-on-Windows

Time efforts: **15** minutes

## Objectives of exercise 

* Download &amp; install Anaconda
* Create Anaconda Environment for R and Python
* Install and run Jupyter Notebook

## Overview of Anaconda

There are several cloud-based data science tools that can make team collaboration more accessible. At times it\'s useful to work directly on your desktop.

Anaconda Distribution is an Open Source distribution of Python and R languages. It comes with a repository of a large number of packages for data science and machine learning, with the most popular and commonly used ones pre-installed. It includes Anaconda Navigator, a graphical interface (GUI) that contains several tools, and IDEs such as Jupyter Notebooks and R Studio. It has binaries for major platforms, including Windows, Linux, and macOS. This lab includes instructions for downloading and installing Anaconda on Windows.

# Exercise 1: Download & Install Anaconda Distribution

**Step 1**: Use the below link to download the Anaconda distribution:

**Link for Download Anaconda Distribution:** https://www.anaconda.com/products/distribution

![Anaconda download](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/1.Anaconda_download.PNG)

***Note**: Depending on your **Operating system**, it would show the download link specific to your OS. Click the **Download** button to download it to your local machine.*

**Step 2**: Once the download completes, right-click the downloaded file and run it as **Administrator**.

![Run as admin](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/2.Run_as_admin.png)

**Step 3**: At the beginning of the welcome window, you need to click **Next** to confirm the installation.

![Confirm installation](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/3.confirm_installation.png)

**Step 4**: Agree to the license.

![License Agreenent](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/4.Agree_license.png)

**Step 5**: In the installation window, select **Just me**, and click **Next**.

![Installation window](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/5.Installation_window.png)

**Step 6**: Select the folder where you would like to **Install Anaconda**, or retain the **Default** installation location and click **Next**.

![Install location](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/6.Location.PNG)

**Step 7**: In the **Advanced Installation Options** window, select **Register Anaconda3 as the default Python 3.9** option, and click **Install**.
 
![Advanced Installation Options](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/7.Install.png)

**Step 8**: You need to wait for the installation to complete. Once installation completes, click **Next**. 

![Installation complete](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/8.Install_click_next.png)

**Step 9**: Click **Next**.

![DataSpell for Anaconda availab-lity](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/9.Click_next.png)

**Step 10**: Click **Finish** to complete the installation of the Anaconda distribution.

![Finish setup](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/10.Finish.png)

# Exercise 2: Create Anaconda Environment

Anaconda environment is a directory containing a specific collection of conda packages you have installed. For example, you may have one environment with NumPy 1.7 and its dependencies and another environment with NumPy 1.6 for legacy testing.

**Ref**: https://conda.io/projects/conda/en/latest/user-guide/concepts/environments.html

**Step 1**: Open the **Anaconda Navigator** from the Windows Start menu.

![Anaconda Navigator (anaconda3) App](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/11.Anaconda_Navigator.png)

![Navigator UI](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/12.Navigator_UI.PNG)

**Step 2**: Create an environment using Anaconda Navigator. Go to the **Environments** tab and click **Create** (at the bottom menu as highlighted below) to create an icon on the Anaconda environment.

![Create icon on Anaconda environment](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/13.Create.png)

**Note**: All the macOS users, select Update index and all your packages will be updated.

***Note**: It is always helpful to create a separate environment because different projects require different packages.* 

**Step 3**: **Give a name** for your environment, select the suitable version and language and click **Create**.

![Create environment and name it](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/14.Create_env.png)

**Note**: The macOS users must uncheck Python and then create the environment.

**Step 4**: Once you create an Anaconda environment, go back to the **Home Page** and **Launch Jupyter** and create a **Python Notebook** (make sure to select the right environment). 

**Note**: The macOS users need to restart their Anaconda prompt first and then launch their Jupyter Notebook.

![Launch jupyter and create Python Notebook](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/15.Launch_jupyter.png)

**Step 5**: This opens **Jupyter Notebook** in the default browser, and now you can select the **kernel** and create a **Notebook**.

![Select kernel and create notebook](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/16.Kernel.png)

# Exercise 3: Create and execute Python Jupyter Notebook

**Step 1**: **Create markdown cells and add text**

In your notebook, **click any code cell**, and in the drop-down menu, change the cell type from Code to Markdown. You will notice that you cannot create Markdown cells without first creating and converting them from Code to Markdown.

![Markdown cell creation](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/17.markdown_creation.png)

In the Markdown cell, write some text like **My First Program**.

To render the Markdown text, make sure the cell is selected (by clicking within it), and press **Play** in the menu or **Shift+Enter**.

 ```
 # My First Program
 ```
 

 Your Markdown cell should now be rendered!

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/18.Md_Output.PNG">

***Note:** To edit your Markdown cell, double-click anywhere within the cell. Note you can use the keyboard shortcut: [m] - Convert Cell to Markdown.*

**Step 2**: **Create new cells**.

* In your Jupyter Notebook, click any of the existing cells to select the cell. 

* Click **Insert Cell Above** or **Insert Cell Below** to insert the cell from the Insert menu. 

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/19.Insert_cell.png" alt="Insert cell">

***Note:** You can use the keyboard shortcuts: [a] - Insert a Cell Above; [b] - Insert a Cell Below.*

**Step 3**: **Write and execute code**.

* In your new empty notebook, click within the gray code cell and write some code, like.

```
1+1
```

* Execute the code by clicking the **Play** button in the menu above the notebook or pressing **Shift+Enter** on your notebook.

* You should see the output 2.

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/20.Code1.PNG" alt="My First Program, output code">

**Step 4**: **Rename, Shutdown kernel, and Save your Notebook**

1 - Click **Rename** from the **File** menu to rename your notebook like ***My_Notebook.ipynb***.

![Rename and Save](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/23.Rename_Save.png)

2 - To shut down the kernel, click **Shutdown** from the **Kernel** menu.

![Shutdown kernel](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/23.Rename_Shutdown.png)

3 - Click **Save Notebook** or **Save Notebook as** to save the notebook from the **File** menu.

![Save notebook](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/23.Save.png)

**Step 5**: **Open the recently created notebook.**

1 - Open **Anaconda Navigator**  from the Windows **Start** menu and **launch Jupyter**.

 ![Launch jupyter notebook](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/15.Launch_jupyter.png)

2 - Go to the **directory** where you **saved** your file and **click** to open it.

 ![Open closed File](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/24.Open_closed_File.png) 

# Practice Exercise

Let us try executing simple math operations 

## Problem 1: Find the minimum and maximum values.

```
x = min(5, 10, 25)
y = max(5, 10, 25)

print(x)
print(y)
```

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/21.Code2.PNG" alt="Minimum and maximum output">

## Problem 2: Find the value of 4 to the power 3.

```
x = pow(4, 3)

print(x)
```

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/22.Code3.PNG" alt="Value of 4 to the power of 3">

# Exercise 4: Create and execute R Jupyter Notebook

Select the **kernel** and create a **Notebook**.

![Open R Notebook](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/25.Open_R_Notebook.png) 

## Problem 1: Find the Multiplication of 2 numbers. 

```
2 * 3 # Multiplication
```

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/27.R_Code2.PNG" alt="Multiplication output">

## Problem 2: Find the Subtraction of 2 numbers.

```
4 - 1 # Subtraction
```

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/28.R_Code3.PNG" alt="Subtraction output">

## Problem 3: Add 2 to the given number. 

```
a <- 1 # Assigning 1 to the variable called "a"
a + 2 # Adding 2
```

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/26.R_Code1.PNG" alt="Adding two to given number output">

## Problem 4: Create a data frame

```
df = data.frame(Emp_Name = c("Jai", "David", "Michael"),
                Job_role = c("Manager", "Team Lead", "Developer" )
               )

print(df)

```

<img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/Installation%20markdowns/Anaconda%20Download%20and%20Installation/images/29.R_Code4.PNG" alt="Data frame output">

Congratulations! You have learned how to download and install Anaconda on your local machine and create a new environment. You have also created a Jupyter Notebook and saved it.

