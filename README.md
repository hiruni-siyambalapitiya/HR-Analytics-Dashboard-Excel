<p align="center">
  <img src="screenshot/HR-Analytics-Dashboard-Banner.png"
       alt="HR Analytics Dashboard Banner"
       width="100%">
</p>

# HR Analytics Dashboard – Employee Attrition Analysis

An end-to-end HR analytics project built **entirely in Excel**. It takes a raw dataset of **1,470 employees and 35 attributes** through data cleaning, validation, feature engineering, pivot analysis and financial analysis, and ends with a dashboard on **why employees leave and what it costs**.

---

## Dashboard Preview

![HR Analytics Dashboard - Excel](assets/dashboard.png)

---

## Presentation

A 7-slide presentation covering the problem, approach, KPIs, findings and recommendations: [`HR_Analytics_Dashboard_Presentation.pptx`](HR_Analytics_Dashboard_Presentation.pptx)

---

## Business Problem

HR leadership wants to understand **employee attrition**:

| # | Question |
|---|----------|
| 1 | How many people are leaving, and is the rate a concern? |
| 2 | Which departments, age groups, experience levels and salary bands are most affected? |
| 3 | How does pay relate to leaving, and what does each department cost? |

---

## Headline KPIs

| KPI | Value |
|-----|-------|
| Total Employees | **1,470** |
| Active Employees | **1,233** |
| Employees Left | **237** |
| Attrition Rate | **16.12%** |
| Average Monthly Salary | **6,502.93** |

---

## Key Insights

| Area | Finding |
|------|---------|
| Age | Attrition is about **36%** for ages 18-25 and falls steadily with age |
| Experience | About **44%** of people with 0-2 years of experience have left |
| Department | **Sales** has the highest rate (about 21%), then Human Resources (about 19%) and R&D (about 14%) |
| Leavers by department | R&D has the most leavers (**133 of 237, 56%**) because it is the biggest department |
| Pay | Leavers earned about **4,787** a month on average against about **6,833** for stayers |
| Salary band | The **Low** band has the highest attrition (about 29%) and the High band the lowest (about 9%) |
| Overtime | About **30%** attrition with overtime against about **10%** without |
| Travel and marital status | Frequent travellers and single employees both leave at about **25%** |

> Percentages are calculated from the `HR_Data` sheet.

---

## Project Structure

| Sheet | Purpose |
|-------|---------|
| `HR_Data` | Original raw dataset (1,470 rows x 35 columns) |
| `Cleaned_Data` | Cleaned data as an Excel Table (`tblHR`) with engineered columns |
| `HR_Analysis` | Data quality report, validation checks and core business KPIs |
| `Pivot_Analysis` | Pivot tables and charts for attrition by department, age, salary and experience |
| `HR_Dashboard` | Final dashboard: KPI cards plus attrition and salary charts |
| `Lookup_Practice` | `XLOOKUP`, `VLOOKUP` and `INDEX/MATCH` demonstrations |
| `HR_Financial_Analysis` | Department salary cost, salary variance vs company average, management summary |

---

## What I Did

### 1. Data cleaning and validation

| Task | Details |
|------|---------|
| Structured table | Converted the data into an Excel Table (`tblHR`) for dynamic ranges and structured references |
| Data quality report | Missing values per column and duplicate employee ID check |
| Validity checks | Invalid-value checks for Attrition, Gender, OverTime, Department and BusinessTravel |
| Range checks | Min/max checks on numeric fields such as Age, MonthlyIncome and DailyRate |

### 2. Feature engineering (calculated columns with `IFS`)

| New column | Logic |
|------------|-------|
| `AgeGroup` | 18-25, 26-35, 36-45, 46-55, 56+ |
| `SalaryBand` | Low, Lower-Middle, Upper-Middle, High (by MonthlyIncome) |
| `ExperienceCategory` | 0-2, 3-5, 6-10, 11-20, 20+ years (by TotalWorkingYears) |
| `TenureCategory` | 0-2, 3-5, 6-10, 11+ years (by YearsAtCompany) |

### 3. Analysis

| Area | What I built |
|------|--------------|
| Pivot analysis | Pivot tables for attrition by department, age group, salary band and experience |
| KPI formulas | `COUNTIF`, `COUNTIFS`, `SUMIFS`, `AVERAGEIFS`, `IFERROR` and `UNIQUE` |
| Financial analysis | Total and average salary cost by department, variance against the company average, highest-attrition and highest-cost departments |
| Lookups | `XLOOKUP`, `VLOOKUP` and `INDEX/MATCH` |

### 4. Dashboard

| Component | Details |
|-----------|---------|
| KPI cards | Total, Active, Left, Attrition Rate and Average Salary |
| Attrition charts | Department, Age Group, Experience and Salary Band vs Attrition |
| Distribution chart | Attrition distribution by department |
| Cost charts | Average and total monthly salary cost by department |

---

## Excel Skills Demonstrated

| Category | Skills |
|----------|--------|
| Data preparation | Excel Tables, Structured References, Power Query, Data Validation Checks |
| Formulas | `IFS`, `COUNTIFS`, `SUMIFS`, `AVERAGEIFS`, `IFERROR`, `UNIQUE` |
| Lookups | `XLOOKUP`, `VLOOKUP`, `INDEX/MATCH` |
| Analysis | Pivot Tables, Pivot Charts, Financial Analysis |
| Reporting | KPI Cards, Dashboard Design |

---

## How to Use

| Step | Action |
|------|--------|
| 1 | Download `HR_Analytics_Project.xlsx` (and `HR_Analytics_Dashboard_Presentation.pptx` for the summary slides) |
| 2 | Open it in **Microsoft Excel 365** or Excel Online (`XLOOKUP`, `IFS` and `UNIQUE` need a recent version) |
| 3 | Start at the `HR_Dashboard` sheet, then explore the other sheets to see how each number is built |

---

## Dataset

The data is the well-known **IBM HR Analytics Employee Attrition** dataset (1,470 employees, 35 fields). It is a fictional dataset created by IBM data scientists and used here for learning and portfolio purposes.

---

## Author

**Hiruni Siyambalapitiya**

[GitHub](https://github.com/hiruni-siyambalapitiya)

