# pewlett-hackard-analysis
----
## Overview of the Analysis
The purpose of this analysis is to determine the number of retiring employees for Pewlett-Hackard and evaluate this number based on different parameters. We are looking at the number of retirees per title, the number of eligible employees for the mentorship program, and also how many roles per department will need to be filled as retirees leave the work force. To do this, we are taking csv files and joining together certain columns to create specific new tables representing these numbers. 

![EmployeeDB](/EmployeeDB.png.png)

This is a visual representation of how the csv files we have on employees relate to each other. 

-------
## Results
- The first table we created was the Retirement Titles table which details the list of employees born from January 1, 1952 and December 31, 1955 who are by definition at retirement age and what their current job title is. There are instances where employees appear multiple times in this list and that is because they could have had multiple titles throughout their careers in the company. This is a result of merging two csv files and filtering the birth dates of the employees.

![retirement_titles_example](/retirement_titles_example.png)

(The table shown is a snippet). 

- The second table, Unique Titles, is one where we have only included the list of retirement age employees who still currently work at the company, and the employees are only listed one time by their most recent title held at the company. 

![unique_titles_example](/unique_titles_example.png) 

(The table shown is a snippet).

- The third table, Retiring Titles, is a step further into the process of determining the count for the number of retirees for each title in the company. The query for this table returned a short table with 2 columns and 7 rows which helps us take a look at the overall picture for how many retirement age people will be leaving the company soon.

![retiring_titles_example](/retiring_titles_example.png)

- The fourth table, Mentorship Eligibility, is taking note of all the employees who are eligible to participate in the mentorship program for training new recruits for the company. 

![mentorship_eligibility_example](/mentorship_eligibility_example.png)

(The table shown is a snippet).

------
## Summary 

How many roles will need to be filled as the "silver tsunami" begins to make an impact?

![roles_tbfilled_example](/roles_tbfilled_example.png)

(The table shown is a snippet).

- Merging the departments table and the retirement_titles tables helped to provide a look at how many people will be leaving the company, which gives us a look at how many roles will need to be replaced over time. 

Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees? 

![mentor_qualified_staff_example](/mentor_qualified_staff_example.png)

This is a filtered table which shows the number of employees in the higher positions in the company who are eligible to mentor other new recruits. We can now compare the previous table with this one to gather insights on the number of retirees available to train. 
