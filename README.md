Power BI Project: Data Professional Survey Visualization Report
Overview
This Power BI project involves analyzing and visualizing a dataset collected from a survey of data professionals. The goal is to gain insights into salary distribution, programming languages used, job roles, and overall job satisfaction.
Steps to follow
Step 1: Load the Data
1.	Download the dataset from the provided source.
2.	Open Power BI Desktop.
3.	Load the dataset into Power BI.
4.	Open the Power Query Editor to clean and transform the data.
Step 2: Data Transformation
1.	Remove Unwanted Columns
o	Delete columns such as Browser, OS, City, Country, and Referrer.
2.	Clean Up Columns
o	Check for and remove unwanted values in the "best_fit_role" column.
o	Split text-based columns using delimiters where needed.
3.	Transform Salary Data
o	Create a new column for average salary.
o	Duplicate the salary column and split values into numeric and non-numeric parts.
o	Replace unwanted characters and clean up values.
o	Compute the average salary using a custom column formula.
4.	Clean Country Data
o	If a country column contains "Other", split it accordingly.
5.	Industry Column Transformation
o	Similar transformations are applied to the industry column.
6.	Apply and Close
o	Once transformations are complete, apply the changes and load the data back into Power BI.
Step 3: Data Visualizations
1. Dashboard Title
•	Add a Text Box with the title: "Data Professional Survey" (Font Size: 36, Bold, Centered)
2. Number of Survey Participants
•	Create a Card visualization.
•	Select the UNIQUE_ID column.
•	Use the Count (Distinct) function and rename it to "Survey Participants".
3. Average Age of Survey Participants
•	Create a Card visualization.
•	Select the CURRENT_AGE column.
•	Use the Average function and rename it to "Average Age".
4. Average Salary by Job Title
•	Create a Stacked Bar Chart.
•	Select job_titles and avg_salary.
•	Use job titles as the legend to display different color patterns.
•	Rename chart and column labels appropriately.
5. Most Popular Programming Languages
•	Create a Clustered Bar Chart.
•	Select fav_programming and UNIQUE_ID.
•	Rename chart and column labels appropriately.
•	Add a title to the legend.
6. Countries of Survey Participants
•	Create a Treemap visualization.
•	Select country as the value and use distinct count.
7. Work-Life Balance Satisfaction
•	Create a Gauge Chart.
•	Select the happy column and configure min, max, and actual values.
8. Salary Satisfaction
•	Create a Donut Chart.
•	Select male, female, and average_salary.
•	Use Average as the function.
Conclusion
This Power BI project provides a structured approach to transforming and visualizing survey data effectively. The final dashboard offers insights into job roles, salary trends, programming languages, and job satisfaction among data professionals.
