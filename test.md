---
layout: page
title: Milanfx Study Notes
permalink: /xxx/
---

Hands-on Lab: Advanced Bash Scripting &quot;}


&lt;p&gt;
    &lt;img src&#x3D;&quot;https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-LX0117EN-SkillsNetwork/images/IDSN-logo.png&quot; width&#x3D;&quot;300&quot; alt&#x3D;&quot;cognitiveclass.ai logo&quot;&gt;
&lt;/p&gt;

Estimated time needed: **30** minutes

Welcome to this hands-on lab, where you will take your Bash scripting chops to the next level. The skills you practice here will serve as logical building blocks for an endless variety of scripting applications. These concepts will also be essential for demonstrating your new skills in the Final Project for this course.

As you develop your Bash scripts, it\&#x27;s always recommended that you test your results at each stage to ensure your logic is behaving as expected. Think of each stage as a building block of your final script that accomplishes an easily digestible sub-task.

## Learning Objectives

After completing this lab, you will be able to:
- Run sets of commands using conditional statements
- Create &#x60;true&#x60;/&#x60;false&#x60; comparisons with logical operators
- Use arithmetic operators to perform basic mathematical calculations
- Use list-like arrays to store and access data
- Execute repetitive tasks with &#x60;for&#x60; loops

## About Skills Network Cloud IDE

Skills Network Cloud IDE (based on Theia and Docker) provides an environment for hands-on labs for course and project related labs. Theia is an open-source IDE (Integrated Development Environment) that can be run on a desktop or on the cloud. To complete this lab, we will be using the Cloud IDE based on Theia running in a Docker container.

## Important notice about this lab environment

Please be aware that sessions for this lab environment are not persisted. Every time you connect to this lab, a new environment is created for you. Any data you may have saved in the earlier session would get lost. Plan to complete these labs in a single session to avoid losing your data.

::page{title&#x3D;&quot;Exercise 1 - Using conditional statements and logical operators&quot;}

In this exercise, you will create a simple Bash script containing a conditional statement to handle the following tasks:

- Prompt the user for a &#x60;Yes&#x60; or &#x60;No&#x60; response to a question
- Print a response based on the user\&#x27;s answer

## 1.1. Create a new Bash script
Create a Bash script file and make it executable.

&lt;details&gt;
&lt;summary&gt;Click here for Hint&lt;/summary&gt;

&gt; Use the &#x60;echo&#x60; command to redirect a **shebang** to a new Bash script.
	
&gt; Alternatively, open a new text file using your favourite text editor and add a **shebang** to it. Remember to make your new script executable.
&lt;/details&gt;

&lt;details&gt;
&lt;summary&gt;Click here for Solution&lt;/summary&gt;
Here&#x27;s a solution using only the command line:  

&#x60;&#x60;&#x60;bash
echo &#x27;#!/bin/bash&#x27; &gt; conditional_script.sh
chmod u+x conditional_script.sh
&#x60;&#x60;&#x60;

&lt;/details&gt;


## 1.2. Query the user and store their response
Now get your script to:
1. Ask the user a binary \&quot;yes or no\&quot; question of your choosing
2. Store the user\&#x27;s answer in a variable.

&lt;details&gt;
&lt;summary&gt;Click here for Hint&lt;/summary&gt;

&gt; Use the &#x60;echo&#x60; and &#x60;read&#x60; commands.

&lt;/details&gt;

&lt;details&gt;
&lt;summary&gt;Click here for Solution&lt;/summary&gt;

&gt; Your Bash script should now look something like this:


&#x60;&#x60;&#x60;bash
#!/bin/bash

echo &#x27;Are you enjoying this course so far?&#x27;
echo -n &quot;Enter \&quot;y\&quot; for yes, \&quot;n\&quot; for no.&quot;
read response
&#x60;&#x60;&#x60;
&lt;/details&gt;


## 1.3. Use a conditional block to select a response for the user
Finally, use a conditional block to print a message to the user based on their response to your query.
&gt; **Tip**: It\&#x27;s best practice to also handle the case where the response doesn\&#x27;t match any of the allowable responses.

&lt;details&gt;
&lt;summary&gt;Click here for Hint&lt;/summary&gt;

&gt; Use a conditional &#x60;if elif else fi&#x60; block that uses a logical operator to compare the user\&#x27;s response to the available response options and prints an appropriate message in each case.

&lt;/details&gt;

&lt;details&gt;
&lt;summary&gt;Click here for Solution&lt;/summary&gt;

&gt; Now your Bash script should be similar to the following:
&#x60;&#x60;&#x60;
#!/bin/bash

echo &#x27;Are you enjoying this course so far?&#x27;
echo -n &quot;Enter \&quot;y\&quot; for yes, \&quot;n\&quot; for no&quot;
read response
if [ &quot;$response&quot; &#x3D; &quot;y&quot; ]
then
    echo &quot;I&#x27;m pleased to hear you are enjoying the course!&quot;
	echo &quot;Your feedback regarding what you have been enjoying would be most welcome!&quot;
elif [ &quot;$response&quot; &#x3D; &quot;n&quot; ]
then
   echo &quot;I&#x27;m sorry to hear you are not enjoying the course.&quot;
   echo &quot;Your feedback regarding what we can do to improve the learning experience&quot;
   echo &quot;for this course would be greatly appreciated!&quot;
else
   echo &quot;Your response must be either &#x27;y&#x27; or &#x27;n&#x27;.&quot;
   echo &quot;Please re-run the script to try again.&quot;
fi
&#x60;&#x60;&#x60;

&lt;/details&gt;



::page{title&#x3D;&quot;Exercise 2 - Performing basic mathematical calculations and numerical logical comparisons&quot;}

In this exercise, you will create a Bash script that performs basic arithmetic calculations on two integers entered by the user. You will also use logical comparisons to determine which calculation leads to the greatest result.

## 2.1. Create a Bash script
Create an executable Bash script that prompts the user for two integers, then stores and prints both the sum and product of the two integers.

&lt;details&gt;
&lt;summary&gt;Click here for Hint&lt;/summary&gt;

&gt; Use the &#x60;echo&#x60; and &#x60;read&#x60; commands as in the previous exercise. 
	
&gt; Recall the notation for arithmetic calculations.

&lt;/details&gt;

&lt;details&gt;
&lt;summary&gt;Click here for Solution&lt;/summary&gt;

&#x60;&#x60;&#x60;
#!/bin/bash

echo -n &quot;Enter an integer: &quot;
read n1
echo -n &quot;Enter another integer: &quot;
read n2

sum&#x3D;$(($n1+$n2))
product&#x3D;$(($n1*$n2))

echo &quot;The sum of $n1 and $n2 is $sum&quot;
echo &quot;The product of $n1 and $n2 is $product.&quot;

&#x60;&#x60;&#x60;
&lt;/details&gt;


## 2.2. Add logic to your script
Add logic to your script that determines whether the sum is greater than, less than, or equal to the product. Display an appropriate statement corresponding to each possible result.

Assume the user inputs two integers. Don\&#x27;t worry about handling the case where the user inputs a non-integer string by mistake.

&lt;details&gt;
&lt;summary&gt;Click here for Hint&lt;/summary&gt;

&gt; Use a conditional block. Recall the notation for logical operators.

&lt;/details&gt;


&lt;details&gt;
&lt;summary&gt;Click here for Solution&lt;/summary&gt;

&#x60;&#x60;&#x60;
#!/bin/bash

echo -n &quot;Enter an integer: &quot;
read n1
echo -n &quot;Enter another integer: &quot;
read n2

sum&#x3D;$(($n1+$n2))
product&#x3D;$(($n1*$n2))

echo &quot;The sum of $n1 and $n2 is $sum&quot;
echo &quot;The product of $n1 and $n2 is $product.&quot;

if [ $sum -lt $product ]
then
   echo &quot;The sum is less than the product.&quot;
elif [ $sum -eq $product ]
then
   echo &quot;The sum is equal to the product.&quot;
elif [ $sum -gt $product ]
then
   echo &quot;The sum is greater than the product.&quot;
fi
&#x60;&#x60;&#x60;
&lt;/details&gt;

::page{title&#x3D;&quot;Exercise 3 -  Using arrays for storing and accessing data within *for* loops&quot;}

In this exercise, you will create a report based on a supplied dataset using the CSV format. You will extract the columns of the dataset into separate arrays and create a new column using arithmetic and array logic. Finally, you will combine the dataset with the new column and save the resulting report as a CSV file.

## 3.1. Download a CSV file to your current working directory
The file, &#x60;arrays_table.csv&#x60;, is located at the following url:

&#x60;&#x60;&#x60;
https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-LX0117EN-SkillsNetwork/labs/M3/L2/arrays_table.csv
&#x60;&#x60;&#x60;

&lt;details&gt;
&lt;summary&gt;Click here for Hint&lt;/summary&gt;

&gt; Use the &#x60;wget&#x60; command.

&lt;/details&gt;

&lt;details&gt;
&lt;summary&gt;Click here for Solution&lt;/summary&gt;
	
&#x60;&#x60;&#x60;
csv_file&#x3D;&quot;https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-LX0117EN-SkillsNetwork/labs/M3/L2/arrays_table.csv&quot;
wget $csv_file
&#x60;&#x60;&#x60;
&lt;/details&gt;

## 3.2. Display the CSV file to understand what it looks like

&lt;details&gt;
&lt;summary&gt;Click here for Hint&lt;/summary&gt;

&gt; Use &#x60;cat&#x60; at the command prompt or open the file using the GUI.

&lt;/details&gt;

&lt;details&gt;
&lt;summary&gt;Click here for Solution&lt;/summary&gt;

&#x60;&#x60;&#x60;
cat arrays_table.csv
&#x60;&#x60;&#x60;
&lt;/details&gt;

## 3.3. Create a Bash script that parses table columns into 3 arrays

&lt;details&gt;
&lt;summary&gt;Click here for Hint&lt;/summary&gt;
	
&gt; Use command substitution, the &#x60;cut&#x60; command, and the notation for creating an array from a list of elements.
&gt;
&gt; Also, print the first array to validate your logic.

&lt;/details&gt;

&lt;details&gt;
&lt;summary&gt;Click here for Solution&lt;/summary&gt;


&#x60;&#x60;&#x60;
#!/bin/bash

csv_file&#x3D;&quot;./arrays_table.csv&quot;

# parse table columns into 3 arrays
column_0&#x3D;($(cut -d &quot;,&quot; -f 1 $csv_file))
column_1&#x3D;($(cut -d &quot;,&quot; -f 2 $csv_file))
column_2&#x3D;($(cut -d &quot;,&quot; -f 3 $csv_file))

# print first array
echo &quot;Displaying the first column:&quot;
echo &quot;${column_0[@]}&quot;
&#x60;&#x60;&#x60;

&lt;/details&gt;

## 3.4. Create a new array as the difference of the third and second columns.
Initialize your new array with a header (a column name), and remember to validate your results.

&lt;details&gt;
&lt;summary&gt;Click here for Hint 1&lt;/summary&gt;
	
&gt; Use a loop to populate your array.

&gt; Determine the number of elements you need and incorporate within your loop statement.
	
&gt; Print both the number of elements and the contents of your new array to validate your logic.
&lt;/details&gt;

&lt;details&gt;
&lt;summary&gt;Click here for Hint 2&lt;/summary&gt;
	
&gt; Recall the &#x60;for&#x60; loop notation when you know the number of iterations needed, and that array indexing starts at 0.
&gt;
&gt; To get the number of lines, use command subsitution on a pipeline that uses the &#x60;cat&#x60; and &#x60;wc&#x60; commands as filters and store the result in a variable.

&lt;/details&gt;

&lt;details&gt;
&lt;summary&gt;Click here for Solution&lt;/summary&gt;

&#x60;&#x60;&#x60;
#!/bin/bash

csv_file&#x3D;&quot;./arrays_table.csv&quot;

# parse table columns into 3 arrays
column_0&#x3D;($(cut -d &quot;,&quot; -f 1 $csv_file))
column_1&#x3D;($(cut -d &quot;,&quot; -f 2 $csv_file))
column_2&#x3D;($(cut -d &quot;,&quot; -f 3 $csv_file))

# print first array
echo &quot;Displaying the first column:&quot;
echo &quot;${column_0[@]}&quot;

## Create a new array as the difference of columns 1 and 2
# initialize array with header
column_3&#x3D;(&quot;column_3&quot;)
# get the number of lines in each column
nlines&#x3D;$(cat $csv_file | wc -l)
echo &quot;There are $nlines lines in the file&quot;
# populate the array
for ((i&#x3D;1; i&lt;$nlines; i++)); do
  column_3[$i]&#x3D;$((column_2[$i] - column_1[$i]))
done
echo &quot;${column_3[@]}&quot;
&#x60;&#x60;&#x60;
&lt;/details&gt;

## 3.5. Create a report by combining your new column with the source table
Save your report as a CSV file.
	
Remember to validate your results.

&lt;details&gt;
&lt;summary&gt;Click here for Hint 1&lt;/summary&gt;
	
&gt; Write the new array to file line-by-line.
	&gt;
&gt; Intitialize the file with a header.

&lt;/details&gt;


&lt;details&gt;
&lt;summary&gt;Click here for Hint 2&lt;/summary&gt;

&gt; Use redirection and recall how to merge two files side-by-side.
&gt;
&gt; Ensure your final report has the correct CSV format.

&lt;/details&gt;

&lt;details&gt;
&lt;summary&gt;Click here for Solution&lt;/summary&gt;

&#x60;&#x60;&#x60;
#!/bin/bash

csv_file&#x3D;&quot;./arrays_table.csv&quot;

# parse table columns into 3 arrays
column_0&#x3D;($(cut -d &quot;,&quot; -f 1 $csv_file))
column_1&#x3D;($(cut -d &quot;,&quot; -f 2 $csv_file))
column_2&#x3D;($(cut -d &quot;,&quot; -f 3 $csv_file))

# print first array
echo &quot;Displaying the first column:&quot;
echo &quot;${column_0[@]}&quot;

## Create a new array as the difference of columns 1 and 2
# initialize array with header
column_3&#x3D;(&quot;column_3&quot;)
# get the number of lines in each column
nlines&#x3D;$(cat $csv_file | wc -l)
echo &quot;There are $nlines lines in the file&quot;
# populate the array
for ((i&#x3D;1; i&lt;$nlines; i++)); do
  column_3[$i]&#x3D;$((column_2[$i] - column_1[$i]))
done
echo &quot;${column_3[@]}&quot;

## Combine the new array with the csv file
# first write the new array to file
# initialize the file with a header
echo &quot;${column_3[0]}&quot; &gt; column_3.txt
for ((i&#x3D;1; i&lt;nlines; i++)); do
  echo &quot;${column_3[$i]}&quot; &gt;&gt; column_3.txt
done
paste -d &quot;,&quot; $csv_file column_3.txt &gt; report.csv
&#x60;&#x60;&#x60;
&lt;/details&gt;



::page{title&#x3D;&quot;Conclusion&quot;}

Congratulations! You have just completed a hands-on lab using advanced Bash scripting logic.
	
In this lab, you learned that you can use:
- Conditional statements to run commands based on whether a specified condition is &#x60;true&#x60; or &#x60;false&#x60;
- Logical operators to make &#x60;true&#x60;/&#x60;false&#x60; operators
- Arithmetic operators  to perform basic mathematical calculations
- List-like arrays to store and access data
- &#x60;for&#x60; loops to execute repetitive tasks


You covered a lot of material here that will be very useful going forward. You will encounter similar problems in your practice and final projects and, best of all, in your career! Remember - you can always come back and review your labs.

&gt; **Tip**: It is worth noting that had we been only interested in efficiency, one of the steps could have been avoided. Specifically, you could have redirected your calculations to a text file line-by-line rather than storing them in an array and then writing the array to file.

Finally, we encourage you to post a review and a rating for this course at any time!
