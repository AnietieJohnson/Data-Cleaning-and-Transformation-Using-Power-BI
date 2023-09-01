# Data Cleaning for Analysis
## Introduction
Data cleaning is not just about making data look better; it's about ensuring accuracy, consistency, and reliability. A clean dataset is a foundation upon which we can build robust analytics, extract meaningful insights, and make informed decisions. In this project, I carried out the process of cleaning and transforming three different datasets using Power BI. I performed series of data preparation steps to ensure that the data is accurate, consistent, and ready for analysis.
## Data Source:
CSV FILE;
- Employee: Containing column names **_empID_**,	**_name_**,	**_Fname_**,	**_dob_**,	**_aadhar_**,	**_city_**,	**_pincode_**, **_phone_**, **_email_**,	**_DeptID_**
- Department: Containing column names **_depID_**,	**_education_**,	**_Designation_**
- Salary: Containing column names  **_empID_**,	**_Base_**,	**_yearly increment_**
## Data Inspection
- Inspected the 'Employee.csv', 'Salary.csv', and 'Department.csv' datasets.
- Identified columns, data types, and potential issues.
## Data Cleaning
1. Loaded each file using **Get data Tab**, I chose _text/csv_
2. I loaded the file into PowerQery Editor for cleaning using Data type detection-: "Based on entire dataset" 
### Employee.csv
- Corrected data types for each columns
- Renamed column headings for consistency
- Checked for missing values, duplicates and Nulls, found none.
- Standardized the **_Date of Birth_** column that had different delimeters seperating the values
- splitted the column to column to enable rearrgngement to suit the format on PowerBi desktop, then I was able to change the data type
### Salary.csv
- Checked for missing values, found none.
- Removed duplicate rows.
- Converted the 'Salary' column to a numeric data type.
- Checked for outliers, decided to keep them.
### Department.csv
- Checked for missing values, found none.
- Removed duplicate rows.
- Renamed columns for clarity.
## Merging Data:
- merged the Employee dataset with Salary Using **_Emp ID_**
- named it Table 1
- then I merged Table 1 and Department dataset using appropriate **_Dept ID_**.
## Conclusion
In conclusion, this task highlight data cleaning and transformation process in Power BI. The documentation outlines each step, ensuring clarity and reproducibility of the process, with a focus on data quality.
