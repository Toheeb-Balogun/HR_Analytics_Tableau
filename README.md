# HR_Analytics_Tableau
HR Analytics Dashboard

# Introduction
As an experienced data analyst, I have been commissioned by XYZ company to help uncover insights and patterns related to the disparities in earnings among groups of employees. Additionally, I will determine whether these discrepancies have an impact on the organization's attrition rate.
**Disclaimer : The data analysis presented herein does not purport to represent the views or opinions of any specific company, and the data set was sourced from the Careerera PGP in Data Science course.**
# Tableau Concepts Applied:
LOD Expression, Calculated Fields, Action and Filters and Data Aggregation.
# Problem Statement
The Stakeholders have requested the following Insights on the dashboard:
•	Count of employee by age group
•	Average income per age
•	Average monthly income
•	Attrition Rate
•	Total Quantity
•	Job Satisfaction
•	Employee count by years worked.
# Data Sourcing
Data was sourced internally. The sourced data is saved electronically on an excel file.
The excel file contains 51486 rows and 35 columns
# Data Transformation/Cleaning :
Some of the transformations that were carried out include:
•	Hierarchy was created to organized data fields such as  Employee number, Age, Gender and age into a logical structure allowing easy navigation.
•	Age group feature was created from employee’s age. The youngest employee is 18 while the oldest is 60 years. The groups that was created is as follows:
o	18-25
o	26-35
o	36-45
o	46-55
o	56-60
•	Calculated field was used to create new fields such as Total number of employees that heave left the organization (Attrition employee count) and Attrition rate using the below formula.
o	IF [Attrition] = "Yes" THEN [Employee Count] ELSE 0 END
o	SUM(attritionemployeecount)/SUM(totalEmployeeCount)

Furthermore, a LOD expression was used to create new fields such as average income at the respective age group level using the below formula:
o	{FIXED [Age (group)]: AVG([Monthly Income])}
o	{FIXED : AVG([MonthlyIncome])}      
# Data Analysis and Visuals
[]
From the Analysis conducted the following insights were gotten
1.	The age of majority of employees fall between the age group 26-45. Similarly, the majority of the employee that have left the organization fall within this same age bracket.
2.	The average income of all employees in the organization is $6796.73.  Age group 46-55 and 56-60 are earning $4425 and $2695 more than average respectivlely. While age group 18-25 are the age group with lowest earning and they earn $3530 less than average.
3.	Majority of employees spend between 1 and 15 years with the organization
4.	The total employee count is 673 with an attrition rate of 12%
# Recommendations
•	Consider provide incentives to facilitate the retention of employees
•	Consider providing more pathways for career advancement
# Limitations to analysis
- There is no specific columns that identify the reasons why employee left the organization.

