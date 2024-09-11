# Bank-Loan-Analysis
## Table of Contents
- [Objectives](#objectives)
- [File in the Repository](#files-in-the-repository)
- [Data Columns](#data-columns)
- [Dashboard Summary](#dashboard-summary)
- [Key Insights](#key-insights)
- [SQL Quesries](#sql-queries)
- [How to use this Repository](#how-to-use-this-repository)
## Objectives
The purpose of this project is to conduct an in-depth analysis of bank loan data to assess loan performance and identify key factors affecting loan outcomes. The analysis helps in understanding loan distribution, repayment trends, loan risk, and borrower characteristics, aiding the bank in making data-driven decisions for loan approvals and risk management.
## Files in the Repository
This repository includes the following files:

- `Bank Loan Analysis.pbix`: A Power BI file containing the loan analysis dashboard with interactive visualizations.
- `Bank Loan REport Query Document.docx`: A Word document that contains all the SQL queries used to retrieve and manipulate the data for analysis.
- `Dashboard Screenshots`: Images of the Power BI dashboard showing key visualizations and insights.
- `README.md`: This file provides an overview of the project, instructions on usage, and insights from the analysis.

## Data Columns
### 1. Date Table

- `Date` : Represents the date of each transaction or record.
- `Month` : Indicates the month of the record.
- `Month Number` : Numeric representation of the month.

### 2. Financial Loan Data

- `address_state` : The state where the loan was applied.
- `annual_income` : Applicant’s annual income.
- `application_type` : Type of loan application (e.g., individual or joint).
- `Avg DTI` : Average Debt-to-Income ratio, a key metric for assessing a borrower's ability to repay.
- `Avg Int Rate` : The average interest rate on loans.
- `Bad Loan %` : The percentage of bad loans out of total loans.
- `Bad Loan Applications` : Number of bad loan applications.
- `Bad Loan Funded Amount` : Total funded amount for bad loans.
- `Bad Loan Received Amount` : Total received amount for bad loans.
- `dti` : Debt-to-Income ratio for a specific record.
- `emp_length` : Length of employment in years.
- `emp_title` : Job title of the applicant.
- `Good Loan %` : Percentage of good loans out of total loans.
- `Good Loan Applications` : Number of good loan applications.
- `Good Loan Funded Amount` : Total funded amount for good loans.
- `Good Loan Received Amount` : Total received amount for good loans.
- `Good v Bad Loan` : A comparison between good and bad loans.
- `grade` : Credit grade assigned to the loan.
- `home_ownership` : Indicates whether the applicant owns a home.

### 3. Loan Status and Application Data

- `id` : Unique identifier for each loan.
- `installment` : The installment payment amount.
- `int_rate` : Interest rate on the loan.
- `issue_date` : The date when the loan was issued.
- `last_credit_pull_date` : Date when the last credit check was performed.
- `last_payment_date` : Date of the last payment made on the loan.
- `loan_amount` : Total loan amount requested.
- `loan_status` : Status of the loan (e.g., fully paid, charged off).
- `member_id` : Unique identifier for the borrower.

### 4. Measures and Aggregated Metrics
- `MoM (Month-over-Month) Metrics` : These are calculated to compare month-to-month changes.

- `MoM Avg DTI` : Month-over-month average Debt-to-Income ratio.
- `MoM Avg Int Rate` : Month-over-month average interest rate.
- `MoM Funded Amount` : Month-over-month funded loan amount.
- `MoM Loan Applications` : Number of loan applications month-over-month.
- `MoM Received Amount` : Amount received from loans month-over-month.
- `MTD (Month-to-Date) Metrics` : These track loan performance from the start of the current month up to the present.

- `MTD Avg DTI` : Month-to-date average Debt-to-Income ratio.
- `MTD Avg Int Rate` : Month-to-date average interest rate.
- `MTD Funded Amount` : Month-to-date funded loan amount.
- `MTD Loan Applications` : Number of loan applications for the current month.
- `MTD Received Amount` : Amount received from loans in the current month.
- `PMTD (Previous Month-to-Date) Metrics` : This compares metrics from the current month to the same point in the previous month.

- `PMTD Avg DTI` : Average Debt-to-Income ratio from the previous month-to-date.
- `PMTD Avg Int Rate` : Average interest rate from the previous month-to-date.
- `PMTD Funded Amount` : Funded amount from the previous month-to-date.
- `PMTD Loan Applications` : Loan applications from the previous month-to-date.
- `PMTD Received Amount` : Amount received from loans in the previous month-to-date.

### 5. Other Measures:

- `Total Funded Amount` : Total amount of money funded for all loans.
- `Total Loan Applications` : Total number of loan applications.
- `Total Received Amount` : Total amount of money received from loans.
- `total_acc` : Total number of accounts held by the applicant.
- `total_paymen` t: Total payments made on loans.
### 6. Loan Purpose and Verification:

- `purpose` : The stated purpose for the loan (e.g., debt consolidation, home improvement).
- `sub_grade` : Sub-grade for the loan, providing more granular credit risk classification.
- `term` : The length of the loan term (e.g., 36 or 60 months).
- `verification_status` : Indicates whether the applicant’s income and employment were verified.
### 7. Select Measures (User-Defined)
These are custom measures that allow you to select, order, and customize fields for specific calculations:
- `Select Measure` : A placeholder to pick a measure.
- `Select Measure Fields` : Allows selection of specific fields to calculate.
- `Select Measure Order` : Allows you to define the order of the measures.

## Dashboard Summary
The Power BI dashboard presents various key performance indicators (KPIs) and metrics related to loan applications, loan statuses, and borrower details. Some of the main sections of the dashboard include:

- **Loan Application Overview**: Visualizations showing the number of loan applications, funded amounts, and the ratio of good vs. bad loans.
- **Loan Risk Metrics**: Displays metrics like Debt-to-Income (DTI) ratios, interest rates, and employment lengths of borrowers to assess loan risks.
- **Loan Performance Trends**: Time-series analysis to track Month-over-Month (MoM) and Year-to-Date (YTD) loan performance in terms of applications and funded amounts.
- **Demographic Breakdown**: Insights into borrower characteristics such as homeownership, employment, and income levels across different states.
- 
## Key Insights
Some of the significant insights from the analysis are:

- **Loan Risk**: Higher interest rates and DTI ratios are associated with a higher likelihood of loan defaults.
- **Geographical Trends**: Certain states have a higher number of loan applications and higher default rates, suggesting regional differences in loan performance.
- **Employment Stability**: Borrowers with longer employment histories are more likely to have successful loan repayments.
- **Seasonal Patterns**: There are noticeable Month-over-Month trends, with certain months showing spikes in loan applications and funded amounts.

## SQL Queries
The SQL queries in the accompanying document were used to extract and transform the data for analysis. The queries focus on:

- Retrieving loan application data by date, state, and borrower details.
- Calculating KPIs such as total loan amounts, funded loans, good vs. bad loans, and borrower credit grades.
- Creating metrics for time-based analysis such as Month-over-Month and Year-to-Date loan performance.

## How to Use This Repository
1. **Power BI Dashboard**: Open the Loan Analysis.pbix file in Power BI Desktop to interact with the dashboard. If you want to explore the data further or customize the visualizations, you can do so within Power BI.

2. **SQL Queries**: The SQL Queries.docx contains all the queries used to generate the dataset. You can run these queries on your SQL database if you want to replicate the data preparation process.
3. **Screenshots**: The screenshots included in the repository provide a quick overview of the key dashboard sections if you don't have access to Power BI.


