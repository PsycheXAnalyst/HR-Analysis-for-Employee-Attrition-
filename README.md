# GROWTH AND PERFORMANCE: Analyzing HR Data to Improve Employee Retention and Performance.

_Project Timeframe: 1/05/2023–05/05/2023_
![](Home_Page_M.jpg)

## INTRODUCTION

Employees are the backbone of any successful organization. Any organization that seeks to achieve its goals and objectives must have talented, reliable and motivated employees. Providing an enabling environment for growth is a key factor that encourages employee engagement and retention is also an essential responsibility of the organization. Every organization at one point in time loses its best talent, however, an organization should take necessary precautions and find the root cause when a significant number of employees are leaving over a certain period of time.

For this project, I worked on an HR dataset that contains the data of past and present employees as well as the administrative data of the organization. As usual, it is always exciting to analyze datasets that will drive real-world impacts. The aim of this project is to gain insights into factors that influence the retention and performance of employees in the organization in order to give recommendations on areas of improvement.

## PROBLEM STATEMENT

One of the biggest challenges facing HR departments today is how to retain and develop top talent.

By analyzing the HR data, I can gain insights into factors that affect employee retention and performance in the company as well as identify areas for improvement.

### Objectives

The objectives are to explore the salary, demographics, hires and terminations and any other areas you deem fit, and provide recommendations to improve employee retention and performance. To achieve this, we will;
- Determine attrition overall attrition rate
- Identify the causes of attrition

## SKILLS DEMONSTRATED

The tool used for the analysis was Microsoft Power BI. The Power BI concepts that were used include;
1. DAX (Data Analysis Expression) Concept for Calculated Measures.
2. Power Query Editor for data cleaning (Conditional Columns and Added Columns)
3. Data Modeling to create a one-to-many relationship between the different tables.

## DATA SOURCING

One of the key parts of the data analysis process is Data Preparation which involves gathering the necessary data to best accomplish the desired analysis. The dataset used for the project was provided by the Human Resources department of the company containing information on Employees, Job Satisfaction, Involvement, Performance, Gender, Education, Department, Hire type, Termination type, etc.

### Data Structure

As a data analyst, I took the time to carefully understand the dataset and planned how to best approach the data cleaning, transformation and analysis process without excluding key features. The HR dataset is structured in the Microsoft Excel workbook (.xlsx) file format. It contains 15 different but related tables, namely:

- Business_Travel: It has 2 columns and 3 rows, and contains the category of travel frequency of employees.
- Department: It has 2 columns and 3 rows, and contains the departments in the company.
- Education: It has 2 columns and 5 rows, and contains the level of education of employees.
- Employee: It has 38 columns and 1,470 rows, and contains the data of employees.
- Employment_Type: It has 2 columns and 2 rows, and contains the employment type of employees.
- Environment_Satisfaction: It has 2 columns and 4 rows, and contains the level of environment satisfaction of employees.
- Gender: It has 2 columns and 3 rows, and contains the gender type of employees.
- Hire_Type: It has 2 columns and 2 rows, and contains the hire type of employees.
- Job_Involvement: It has 2 columns and 4 rows, and contains the level of involvement of employees.
- Job_Role: It has 2 columns and 9 rows, and contains the job roles of employees.
- Job_Satisfaction: It has 2 columns and 4 rows, and contains the level of job satisfaction of employees.
- Performance: It has 2 columns and 4 rows, and contains the performance level of employees.
- Relationship_Satisfaction: It has 2 columns and 4 rows, and contains the relationship satisfaction level of employees.
- Termination_Type: It has 2 columns and 2 rows, and contains the job termination type of employees.
- Work_Life_Balance: It has 2 columns and 2 rows, and contains the quality of the work-life balance of employees.

## DATA TRANSFORMATION

Before commencing any analysis, the HR dataset was imported into Power Query on Microsoft Power BI.
Data cleaning is a key aspect of the data processing stage as it ensures data accuracy and credibility. Here, you can understand the data and identify inconsistencies.
The following transformations were done:

1. Removal of errors and duplicates present in the data for each table and column.
2. Check for blank cells or missing values in the dataset.
3. Correction of data types, especially dates.
4. Reduction of decimal places in columns having currency values.

![](POwer_Query.jpg)


_Power Query View_

Now that our data is squeaky clean, let’s jump into Power BI properly!

## MODELLING

I discovered that 14 tables out of all 15 available tables in the dataset had columns that were related to the “Employee” table. These columns served as the Foreign Keys for the fact (Employee) table. A one-to-many relationship was created to model the fourteen (14) tables together for easy analysis and visualization.

![](Data_Model_M.jpg)


_A Star-Schema Data Model_

## ANALYSIS AND VISUALIZATIONS

In this step, we carried out an exploratory analysis of the data to answer the questions that were stated earlier.

First of all, I did a quick summary by calculating some important measures using DAX.

![](Measures_M.jpg)

_Calculated Measures_

![](KPI_Summary_M.jpg)


_Key Measures_

The visuals above show that out of 1,470 employees, only 1,233 are active employees giving an attrition rate of 16% (237). Also, there were more male employees than the females in the company having had 265 new hires at present.

### Question 1
What is the age distribution and gender of employees?

![](Age_Gender.jpg)


_Employees by Age Group & Gender_

This organization has an active workforce. More than 50% of its employees fall within the age bracket of 26–45 years and these are active work years.

### Question 2
What is the attrition trend amongst different departments and education levels?

![](Department_Education_M.jpg)


_Attrition by department & education level_

Next, I moved on to the attrition analysis. Research & Development department (133) had the highest number of attrition over the years followed by the Sales department (92). The majority of those employees had a Bachelor’s degree (99).

### Question 3
What is the attrition trend between males and females?

![](Attrition_gender.jpg)


_Attrition by Gender_

### Question 4
What is the attrition trend by distance status?

![](Distance_Status.jpg)


_Attrition by distance status_

With regards to the distance to the company, the majority (60.76%) of attritions lived near (<10 miles) the company followed by those that lived far (>10 miles).

### Question 5
Did employees leave voluntarily or involuntarily?

![](Termination_Type.jpg)


_Attrition by Termination types_

Voluntary attrition was the highest. This could result from a number of factors like low pay, poor working conditions, and lack of career growth.

### Question 5
Is performance indicators like Job Involvement, Job Satisfaction, and Performance Rating low amongst employees that left?
