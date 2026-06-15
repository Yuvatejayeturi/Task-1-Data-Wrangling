# Netflix Data Wrangling Project
## ApexPlanet Data Analytics Internship - Task 1
### Project Overview
This project focuses on data cleaning, preprocessing, and transformation of the Netflix Movies and TV Shows dataset. The objective is to identify data quality issues, perform necessary cleaning operations, and prepare an analysis-ready dataset for future Exploratory Data Analysis (EDA) and Business Intelligence tasks.
---
## Objective
The primary goals of this project are:
* Understand the structure of the dataset
* Assess data quality issues
* Handle missing values
* Perform data transformation
* Create useful derived features
* Generate a clean dataset ready for analysis
---
## Dataset Information
| Attribute     | Value                       |
| ------------- | --------------------------- |
| Dataset Name  | Netflix Movies and TV Shows |
| Total Records | 8807                        |
| Total Columns | 12                          |
| File Format   | CSV                         |
### Dataset Columns
* show_id
* type
* title
* director
* cast
* country
* date_added
* release_year
* rating
* duration
* listed_in
* description
---
## Tools & Technologies Used
* Python
* Pandas
* Jupyter Notebook
* GitHub
---
## Data Quality Assessment
### Missing Values Detected
| Column     | Missing Values |
| ---------- | -------------- |
| director   | 2634           |
| cast       | 825            |
| country    | 831            |
| date_added | 10             |
| rating     | 4              |
| duration   | 3              |
### Duplicate Records
* Duplicate Rows Found: 0
---
## Data Cleaning Process
The following preprocessing steps were performed:
### 1. Missing Value Handling
* Filled missing values in `director` with "Unknown"
* Filled missing values in `cast` with "Unknown"
* Filled missing values in `country` with "Unknown"
* Handled missing values in `rating`
* Handled missing values in `duration`
### 2. Data Type Conversion
* Converted `date_added` column to datetime format
### 3. Feature Engineering
Created a new column:
* `content_age` = Current Year − Release Year
This feature helps analyze the age of content available on Netflix.
---
## Project Structure
```text
Task1-Data-Wrangling/
│
├── netflix_titles.csv
├── cleaned_dataset.csv
├── Data_Dictionary.xlsx
├── data_cleaning.ipynb
└── README.md
```
---
## Files Included
### netflix_titles.csv
Original raw dataset.
### cleaned_dataset.csv
Final cleaned dataset after preprocessing.
### Data_Dictionary.xlsx
Detailed explanation of all dataset columns and their data types.
### data_cleaning.ipynb
Jupyter Notebook containing all cleaning and transformation steps.
### README.md
Project documentation.
---
## Key Outcomes
* Successfully identified and resolved data quality issues.
* Removed inconsistencies and handled missing values.
* Converted date fields into proper format.
* Created a new analytical feature (`content_age`).
* Generated a clean dataset ready for Exploratory Data Analysis (EDA).
---
## Future Work
The cleaned dataset will be used in the next internship task:
* Exploratory Data Analysis (EDA)
* Data Visualization
* SQL-Based Business Analysis
* Dashboard Development
---
## Author
**Yuva Teja**
Data Analytics Intern
ApexPlanet Software Pvt. Ltd.
