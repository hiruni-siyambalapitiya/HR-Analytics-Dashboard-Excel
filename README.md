<p align="center">
  <img src="screenshot/HR-Analytics-Dashboard-Banner.png"
       alt="HR Analytics Dashboard Banner"
       width="100%">
</p>

# HR Analytics Dashboard – Employee Attrition Analysis
An end-to-end HR analytics project built entirely in Excel. It takes a raw dataset of 1,470 employees and 35 attributes through data cleaning, validation, feature engineering, pivot analysis and financial analysis, and ends with an interactive dashboard on why employees leave and what it costs.

## Dashboard Preview
HR Analytics Dashboard - Excel

## Presentation
A 7-slide presentation summarising the problem, approach, KPIs, key findings and recommendations is included in this repository: HR_Analytics_Dashboard_Presentation.pptx.

## Business Problem
HR leadership wants to understand employee attrition:

How many people are leaving, and is the rate a concern?
Which departments, age groups, experience levels and salary bands are most affected?
How does pay relate to leaving, and what does each department cost?

## Headline KPIs
|KPI	     |                Value|
Total Employees	         1,470
Active Employees	       1,233
Employees Left	         237
Attrition Rate	         16.12%
Average Monthly Salary	 6,502.93

## Key Insights

Early-career and low-tenure staff leave the most. Attrition is about 36% for ages 18-25 and about 44% for people with 0-2 years of total experience.
It falls steadily with age and experience.
Sales has the highest attrition rate (about 21%), followed by Human Resources (about 19%). Research & Development has the lowest rate (about 14%) but the largest number of leavers (133 of 237, 56%) because it is the biggest department.
Pay matters. Leavers earned about 4,787 per month on average, against about 6,833 for those who stayed. The Low salary band loses the highest share of its people.
Overtime is a strong signal. Attrition is about 30% for employees working overtime, against about 10% for those who do not.
Frequent travel and being single also show higher attrition (about 25% for both groups).

Percentages are calculated from the HR_Data sheet.

## Project Structure
Sheet	                  Purpose
HR_Data	                Original raw dataset (1,470 rows x 35 columns)
Cleaned_Data	          Cleaned data as an Excel Table (tblHR) with engineered columns
HR_Analysis	            Data quality report, validation checks and core business KPIs
Pivot_Analysis	        Pivot tables and charts for attrition by department, age, salary and experience
HR_Dashboard	          Final dashboard: KPI cards plus attrition and salary charts
Lookup_Practice	        XLOOKUP, VLOOKUP and INDEX/MATCH demonstrations
HR_Financial_Analysis	  Department salary cost, salary variance vs company average, management summary

## What I Did
1. Data cleaning and validation
 Converted the data into a structured Excel Table (tblHR) for dynamic ranges and structured references.
 Built a data quality report: missing values per column, duplicate employee IDs, and invalid-value checks for fields such as Attrition, Gender, OverTime,   Department and BusinessTravel.
 Ran min/max range checks on numeric fields (Age, MonthlyIncome, DailyRate and others).

2. Feature engineering (calculated columns with IFS)
   New column	              Logic
    AgeGroup	              18-25, 26-35, 36-45, 46-55, 56+
    SalaryBand	            Low, Lower-Middle, Upper-Middle, High (by MonthlyIncome)
    ExperienceCategory	    0-2, 3-5, 6-10, 11-20, 20+ years (by TotalWorkingYears)
    TenureCategory	        0-2, 3-5, 6-10, 11+ years (by YearsAtCompany)

   
3. Analysis
 Pivot tables for attrition by department, age group, salary band and experience.
 KPI formulas with COUNTIF, COUNTIFS, SUMIFS, AVERAGEIFS, IFERROR and UNIQUE.
 Financial analysis of total and average salary cost by department, variance against the company average, and highest-attrition / highest-cost departments.
 Lookup functions with XLOOKUP, VLOOKUP and INDEX/MATCH.

4. Dashboard
KPI cards: Total, Active, Left, Attrition Rate and Average Salary.
Charts: Department vs Attrition, Age Group vs Attrition, Experience vs Attrition, Salary Band vs Attrition, attrition distribution by department, and average and total salary cost by department.

## Excel Skills Demonstrated

Excel Tables · Structured References · Pivot Tables & Pivot Charts · Power Query 
· IFS · COUNTIFS / SUMIFS / AVERAGEIFS · XLOOKUP / VLOOKUP / INDEX-MATCH · UNIQUE 
· Data Validation Checks · Dashboard Design

## How to Use

Download HR_Analytics_Project.xlsx from this repository (and HR_Analytics_Dashboard_Presentation.pptx for the summary slides).
Open it in Microsoft Excel 365 (or Excel Online). XLOOKUP, IFS and UNIQUE need a recent Excel version.
Start at the HR_Dashboard sheet, then explore the other sheets to see how each number is built.

## Dataset
The data is the well-known IBM HR Analytics Employee Attrition dataset (1,470 employees, 35 fields). It is a fictional dataset created by IBM data scientists and is used here for learning and portfolio purposes.

## Tools & Technologies

- Microsoft Excel 365
- Excel Tables
- Excel Formulas and Functions
- PivotTables
- PivotCharts
- Data Cleaning and Validation
- Data Visualization


## Author

**Hiruni Siyambalapitiya**

BSc (Hons) in Information Technology – SLIIT

GitHub: [hiruni-siyambalapitiya](https://github.com/hiruni-siyambalapitiya)
