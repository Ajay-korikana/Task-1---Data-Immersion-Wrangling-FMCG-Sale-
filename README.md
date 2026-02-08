# Task-1---Data-Immersion-Wrangling-FMCG-Sale-
Performed data immersion and wrangling on an FMCG sales dataset by profiling the data, identifying quality issues such as missing values, duplicates, and inconsistent formats, and resolving them using Python (Pandas). Delivered a clean, validated, analysis-ready dataset.


Task-1: Data Immersion & Wrangling


Objective:- 
The objective of this task is to gain a deep understanding of the provided dataset and perform the critical first step of data analysis: data acquisition, quality assessment, cleaning, and preparation.
The final output is a clean, structured, and analysis-ready dataset suitable for downstream analytics and visualization.


 Dataset Overview: 
•	Domain: FMCG Sales Transactions
•	Granularity: One row represents a single product (SKU) sold within an invoice
•	Source: Internal transactional dataset (provided)


The dataset contains information related to:
•	Invoices and transactions
•	Customers and geography
•	Products and quantities
•	Pricing, discounts, and tax components


Tools & Technologies Used:  
•	Python
•	Jupyter Notebook
•	Pandas
•	Excel

 Data Quality Issues Identified:-
During initial data profiling and exploration, the following data quality issues were identified in the dataset:

1.Missing (Null) Values: 
•	Several columns contained null or missing values
•	Nulls were observed mainly in:
o	Customer-related fields (e.g., customer name, GSTIN)
o	Tax components (CGST, SGST/UTGST, IGST, CESS, Additional CESS)
•	Missing values in tax totals required derivation from individual tax components
Impact:
Missing values can distort revenue, tax, and customer-level analysis if not handled properly.


2.Duplicate Records: 
•	Duplicate records were found at the invoice–item level
•	Duplicates were identified using combinations of:
o	Invoice Number
o	Item Code
Impact:
Duplicates can lead to overstated sales, quantities, and tax amounts.


3.Inconsistent Column Naming: 
•	Column names were:
o	Lengthy
o	Inconsistent in format
o	Not SQL-friendly
•	Issues included:
o	Mixed casing
o	Spaces and special characters
o	Non-standard naming conventions
Impact:
Inconsistent column names reduce code readability and increase error risk during analysis.


4.Incorrect Data Types: 
•	Date columns were not consistently stored as datetime objects
•	Numeric fields (prices, amounts, taxes) were sometimes stored as text
•	Presence of formatting characters (commas, symbols) in numeric columns
Impact:
Incorrect data types prevent accurate calculations and aggregations.


5.Incomplete Tax Group Values: 
•	tax_group_value contained null values
•	Individual tax components (CGST, SGST/UTGST, IGST, CESS, Additional CESS) were present
Impact:
Tax totals could not be directly used and required recalculation.



 Task Breakdown:-
 
1.Data Access & Familiarization:
•	Loaded raw data into Python using Pandas
•	Preserved raw data integrity by working on a copy
•	Reviewed schema, column names, and data types
•	Created a data dictionary to document column meanings


2.Data Quality Assessment:
Performed initial data profiling to identify:
•	Missing (null) values
•	Duplicate records
•	Incorrect data types (dates, numeric fields)
•	Inconsistent formats
•	Potential outliers in quantity and monetary values
All issues were documented before cleaning.


3.Data Cleaning & Transformation: 
Implemented data cleaning using Python (Pandas):
•	Standardized date formats
•	Converted numeric columns safely
•	Handled missing values using logical business rules
•	Removed duplicate records where applicable
•	Renamed columns to clean, consistent, and SQL-friendly names
•	Validated tax calculations (CGST, SGST, IGST, CESS)
•	Ensured schema consistency after transformations


4.Feature Preparation: 
Prepared the dataset for analysis by:
•	Ensuring transaction-level accuracy
•	Validating invoice-level totals
•	Making the dataset suitable for SQL, EDA, and dashboards


 Deliverables: 
•	Cleaned dataset (.xlsx)
•	Python cleaning script (Jupyter Notebook)
•	 Data dictionary
•	 Reproducible and well-documented workflow



Key Learnings: 
•	Importance of data understanding before analysis
•	Handling real-world data quality issues
•	Writing clean, reproducible data cleaning code
•	Maintaining professional data workflows


Next Steps: 
•	Exploratory Data Analysis (EDA)
•	SQL-based analytics
•	Dashboard creation (Power BI / Tableau)
•	Advanced analytics and forecasting
________________________________________
 Author
Ajay Korikana
Data Analytics | Business Analytics
(Project completed as part of experiential learning / internship task)
