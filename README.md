# Data Cleaning for Analysis
## Introduction
Data cleaning is not just about making data look better, it's about ensuring accuracy, consistency, and reliability. A clean dataset is a foundation upon which we can build robust analytics, extract meaningful insights, and make informed decisions. In this task, I carried out the process of cleaning and transforming three different datasets using Power BI. I performed series of data preparation steps to ensure that the data is accurate, consistent, and ready for analysis.
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
- Corrected data types for each column
- Renamed column headings for clarity and consistency
- Checked for missing values, duplicates and Nulls, found none.
- Standardized the **_Date of Birth_** column that had different delimeters seperating the values
- Splitted the column to suit the date format on PowerBi desktop, then I was able to change the data type.

DATASET BEFORE CLEANING         |        DATASET AFTER CLEANING
:-------------------------------:|:---------------------------------:
![](https://github.com/AnietieJohnson/Data-Cleaning-and-Transformation-Using-Power-BI/blob/main/employee%20csv%20dataset%20before%20cleaning.png) | ![](https://github.com/AnietieJohnson/Data-Cleaning-and-Transformation-Using-Power-BI/blob/main/Employee%20Data%20set%20after%20cleaning.png)
### Salary.csv
- Corrected data types for each column
- Renamed column headings for Clarity and consistency
- Checked for missing values and duplicates, there was none
- For the Nulls present I used **_Keep rows tab_** from **HOME** to keep the 100 valid rows and removed the 99 rows of nulls

DATASET BEFORE CLEANING        | DATASET AFTER CLEANING
:-------------------------------:|:------------------------------:
![](https://github.com/AnietieJohnson/Data-Cleaning-and-Transformation-Using-Power-BI/blob/main/Salary%20CSV%20dataset%20before%20cleaning.png) | ![](https://github.com/AnietieJohnson/Data-Cleaning-and-Transformation-Using-Power-BI/blob/main/salary%20dataset%20after%20cleaning.png)
### Department.csv
- Corrected data types for each column
- Renamed column headings for Clarity and consistency
- Checked for missing values and duplicates, there was none
- For the Nulls present I used **_Keep rows tab_** from **HOME** to keep 11 valid rows and removed nulls and empty cells.

DATASET BEFORE CLEANING       |  DATASET AFTER CLEANING
:-------------------------------:|:--------------------------------:
![](https://github.com/AnietieJohnson/Data-Cleaning-and-Transformation-Using-Power-BI/blob/main/department%20csv%20data%20set%20before%20cleaning.png) | ![](https://github.com/AnietieJohnson/Data-Cleaning-and-Transformation-Using-Power-BI/blob/main/deptid.png)

## Data Integrity
I checked column quality, column profile and column distribution for each column in each file;
- This helps to identify and address issues like missing values, outliers, and inconsistencies, ensuring data reliability.
- It also enhance data quality and trustworthiness for accurate insights and visualizations.
## Merging Data:
USED the left outer Join to
- Merged the Employee dataset with Salary Using **_EmpID_** 
- Named it Table 1
- Then I merged Table 1 and Department dataset using **_DepID_**.

**DATASET AFTER MERGE**
![](https://github.com/AnietieJohnson/Data-Cleaning-and-Transformation-Using-Power-BI/blob/main/merge%20datasets%20using%20left%20outer%20join.png)

## Conclusion
In conclusion, this task highlight data cleaning and transformation process in Power BI. The documentation outlines each step, ensuring clarity and reproducibility of the process, with a focus on data quality.
