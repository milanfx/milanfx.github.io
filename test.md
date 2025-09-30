---
layout: page
title: Milanfx Study Notes
permalink: /xxx/
---


# Getting Started with IDE 

**Estimated Time Needed: 15 Minutes**

### Overview

In this lab, you will become familiar with using an Integrated Development Environment (IDE). The IDE you will be using is Skills Network Cloud IDE, based on an open-source project called Theia.  This IDE is similar to the popular Visual Studio (VS) Code IDE. In this lab, you will explore the IDE and use it to create and run a simple Python program. You will install a library, create a code file, save it, and edit it to make changes.

### Objectives

- Explore the IDE interface.
- Install a package using terminal.
- Create a simple Python program using the IDE.
- Execute the program.
- Edit the source code and re-run the program.

### Environment

**Two Components of the Skills Network Lab environment:**

- The instructions that you will follow to complete this lab are displayed on the left side of the screen.

- The area on the right side of the screen is the actual IDE, where you will use the menus, terminals, and tools to develop your code.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/labs/v1/labs/images/ide.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div> 

## Exercise 1: Explore the IDE interface

### Explore the menus, terminals, and tools

Let us now explore the IDE interface. Please click on each of the icons and menu items highlighted in red boxes in the following screenshots to become familiar with their purpose.

**Step 1:** In the **Explorer** menu, you will find your folders, files (created or cloned), and pre-requisites installed.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/labs/v1/labs/images/explorer.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div> 

**Step 2:** In the **Search** menu, you can search for particular folders or files that were created or cloned.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/labs/v1/labs/images/search.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div> 

**Step 3:** In the **Source Control** menu, you will find the cloned repository.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/labs/v1/labs/images/source_control.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div> 

**Step 4:** In the **Debug** menu, you can debug and troubleshoot your code.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/labs/v1/labs/images/debug.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div> 

**Step 5:** In the **Extensions** menu, you can check the recommended, installed, and built-in software already provided as the pre-requisitesprerequisites. 

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/labs/v1/labs/images/extention.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div> 

**Step 6:** In the **Skills Network Toolbox**, you will find options to use database, big data, cloud, and other tools to complete lab exercises in other courses.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/labs/v1/labs/images/toolbox.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div> 

**Step 7:** Explore the menu options at the top of the IDE: File, Edit, Selection, View, Go, Run, Terminal, Help. You will be using some of these menu items in subsequent exercises. A summary of what they are used for is provided below.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/labs/v1/labs/images/menu.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div> 

- **File:** This menu is used to create a new file or folder and save the file.

- **Edit:** This menu is used to undo, redo, cut, paste, and find the file.

- **Selection:** This menu is used to Select All, Copy line up or down and Move line up or down in the file.

- **View:** This menu is used to view the other menus like explorer, extensions, and search.

- **Go:** This menu is used to Go back, view the last edit location, and go to the files.

- **Run:** This menu is used for debugging and Adding configurations.

- **Terminal:** This menu is used to open the New terminal and run the tasks.

- **Help:** This menu is used to view the list of extensions and get started a file.

Click on each menu and explore them.

**You will learn about folder and file creation and how to use the terminal to run the commands later in this lab.**

## Exercise 2: Create a simple Python program using the IDE

**Step 1:** On the window to the right, click on the File menu and select **"New Folder"** option, as shown in the image below.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/labs/v1/labs/images/folder.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div> 

Name the folder **"welcome101"**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/labs/v1/labs/images/folder_2.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div> 

**NOTE:** Ensure that the folder is created within the /home/project directory. If you\'re encountering any issues, right-click on an empty area and select New Folder*

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/VQca0p7KO2XuK9DXXQy5AA/new-folder-2.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div> 

**Step 2:** Right-click on the folder welcome101 and click on **"New File"**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/labs/v1/labs/images/file.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div>

Create a new file and name it **"welcome.py"**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/labs/v1/labs/images/file2.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div>

**Step 3:** Paste the below code to the welcome.py file and save it using Ctrl+S.

```Python
import numpy as np

a = np.array([1,2])
b = np.array([3,4])
c = a + b
print(c)
```

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/images/welcome_py.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div>

## Exercise 3: Execute the program

**Step 1:** Open a terminal window using the editor New  Terminal.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/labs/v1/labs/images/new-terminal.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div>

In the terminal, you will run all the commands to complete the lab.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/labs/v1/labs/images/terminal1.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div> 

**Step 2:** Verify that python is installed.

```bash
python3.11 --version
```

You should see output similar to this, though the versions may be different:

```
Python 3.11.11
```

**Step 3:** Install the numpy package.

```bash
python3.11 -m pip install numpy
```
You should see the an output similar to this.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/images/numpy_install.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div>

**Step 4:** Change the directory for this lab by using the command shown below in the terminal.

```bash
cd welcome101
```

**Step 5:** Run the program in the terminal using the below command:

```bash
python3.11 welcome.py
```

**You will get the following output!**

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/images/code_output.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div>

## Exercise 4: Edit the source code and re-run the program

**Step 1:** Replace the source code with the code shown below:

```python
message= "Welcome to the world of programming!"
print (message)
```

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/labs/v1/labs/images/correct_code.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div> 

**Step 2:** Run the program in the terminal using the command below:

```bash
python3.11 welcome.py
```

You should see an output similar to this.

```
Welcome to the world of programming!
```

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/labs/v1/labs/images/correct_output.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div>

## Practice Exercises

**Step 1:** Create a new folder called "software101".

<details>
<summary>Click here for Hint</summary>

On the window to the right, click on the File menu and select the **"New Folder"** option, as shown in the image below. Name the folder **"software101"**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/labs/v1/labs/images/folder.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div>

</details>

**Step 2:** In software101, create a new file called "software.py".

<details>
<summary>Click here for Hint</summary>

Right-click on the folder software101, click on **"New File"**, create a new file, and name it **"software.py"**.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/labs/v1/labs/images/hint.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div>

</details>

**Step 3:** Write code to add two arrays using Numpy library.

- NOTE: Since the library is already installed in the practice, there is no need to install it again.

<details>
<summary>Click here for Hint</summary>

Import the numpy library, create two numpy arrays, and add them.
</details>

<details>
<summary>Click here for Solution</summary>

Paste the code below to the software.py file and save it using Ctrl+S.

```Python
import numpy as np

a = np.array([2,3,4])
b = np.array([3,2,1])
c = a + b
print (c)
```

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/images/image_1.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div>

</details>

**Step 4:** Run the program.

<details>
<summary>Click here for Solution</summary>

Run the program in the terminal using the below command. Make sure you are in the correct folder.

```bash
cd software101
python3.11 software.py
```

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/images/image_2.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div>

</details>

**Step 5:** Edit the software.py file and change one of the arrays.

<details>
<summary>Click here for Solution</summary>

Change the array 'a' to [5,3,1] and save the file.

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/images/image_3.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div>

</details>

**Step 6:** Run the updated file.

<details>
<summary>Click here for Solution</summary>

Run the program in the terminal using the below command:

```bash
python3.11 software.py
```

<div align="center"><div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0224EN-Coursera/images/image_4.png" style="width:880px; max-height:580px; object-fit:contain;"></div></div>

</details>

**Congratulations!** 

You have completed this lab and know how to run python programs in an IDE.






