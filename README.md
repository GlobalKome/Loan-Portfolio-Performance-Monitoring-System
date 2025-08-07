# Loan-Portfolio-Performance-Monitoring-System
This project aims to develop a comprehensive dashboard suite to monitor the health and performance of the bank’s loan portfolio across customer segments and time periods.  
✅ Real-World Value: Helps executives monitor the profitability and risk exposure of the loan book.

# Table of Contents
- [Executive Summary](#executive-summary)
- [Objective](#objective)
- [User Story](#user-story)
- [Design](#design)
     - [Dashboard Component Requirements](#dashboard-component-requirements)
     - [Summary Dashboard](#summary-dashboard)
     - [Overview Dashboard](#overview-dashboard)
     - [Details Dashboard](#details-dashboard)
- [Tools](#tools)
- [Data Exploration Notes](#data-exploration-notes)
- [Testing](#testing)
- [Visualization](#visualization)
   - [Results](#results)
- [Recommendations](#recommendations)
- [Conclusion](#conclusion)

# Executive Summary
ZenithCore Bank aims to enhance visibility into its expanding retail loan portfolio. This project provides an interactive dashboard suite that enables executive leadership and lending teams to monitor loan applications, assess repayment performance, and proactively manage risk exposure. The solution enhances data-driven decision-making by offering clear insights through three tailored dashboards: Summary, Overview, and Details.

# Objective
  - Develop dynamic dashboards to track retail loan KPIs
  - Identify underperforming loan segments early
  - Provide clear, actionable insights to different stakeholders
  - Enable executive reporting with minimal manual input
  - Improve efficiency in loan performance monitoring

# User Story
Mrs. Adaobi Okonkwo, the Head of Retail Lending at ZenithCore Bank, is responsible for overseeing the performance of thousands of consumer loans issued by the bank. With limited visibility into how these loans are performing across customer types, states, and purposes, she needs an efficient way to track loan application trends, repayment patterns, and risk indicators in one place.

To solve this, she contracted me, a data analyst, to develop a Loan Portfolio Performance Monitoring System made up of three dashboards:
  A Summary Dashboard for executive insights,
  An Overview Dashboard to explore trends by segment,
  A Details Dashboard for operational-level tracking.

These tools will empower her team to shift from reactive reporting to proactive, insight-driven portfolio management—ultimately enabling smarter lending strategies and minimizing exposure to high-risk borrowers.

# Design
## Dashboard Component Requirements
### Summary Dashboard
- Total Loan Applications: We need to calculate the total number of loan applications received during a specified period. Additionally, it is essential to monitor the Month-to-Date (MTD) Loan Applications and track changes Month-over-Month (MoM).
- Total Funded Amount: Understanding the total amount of funds disbursed as loans is crucial. We also want to keep an eye on the MTD Total Funded Amount and analyse the Month-over-Month (MoM) changes in this metric.
- Total Amount Received: Tracking the total amount received from borrowers is essential for assessing the bank's cash flow and loan repayment. We should analyse the Month-to-Date (MTD).
- Total Amount Received and observe the Month-over-Month (MoM) changes.
- Average Interest Rate: Calculating the average interest rate across all loans, MTD, and monitoring the Month-over-Month (MoM) variations in interest rates will provide insights into our lending portfolio's overall cost.
- Average Debt-to-Income Ratio (DTI): Evaluating the average DTI for our borrowers helps us gauge their financial health. We need to compute the average DTI for all loans, MTD, and track Month-over-Month (MoM) fluctuations.

Good Loan v Bad Loan KPI’s

| Good Loan | Bad Loan|
| --- | --- | 
| Good Loan Application Percentage | Bad Loan Application Percentage |
| Good Loan Applications | Bad Loan Applications |
| Good Loan Funded Amount | Bad Loan Funded Amount |
| Good Loan Total Received Amount | Bad Loan Total Received Amount |

Loan Status Grid View

In order to gain a comprehensive overview of our lending operations and monitor the performance of loans, we aim to create a grid view report categorized by 'Loan Status.’ By providing insights into metrics such as 'Total Loan Applications,' 'Total Funded Amount,' 'Total Amount Received,' 'Month-to-Date (MTD) Funded Amount,' 'MTD Amount Received,' 'Average Interest Rate,' and 'Average Debt-to-Income Ratio (DTI),' this grid view will empower us to make data-driven decisions and assess the health of our loan portfolio.

### Overview Dashboard
CHARTS
- Monthly Trends by Issue Date (Line Chart):  To identify seasonality and long-term trends in lending activities
- Regional Analysis by State (Filled Map): To identify regions with significant lending activity and assess regional disparities
- Loan Term Analysis (Donut Chart): To allow the client to understand the distribution of loans across various term lengths.
- Employee Length Analysis (Bar Chart): How lending metrics are distributed among borrowers with different employment lengths, helping us assess the impact of employment history on loan applications.
- Loan Purpose Breakdown (Bar Chart): Will provide a visual breakdown of loan metrics based on the stated purposes of loans, aiding in the understanding of the primary reasons borrowers seek financing.
- Home Ownership Analysis (Tree Map): For a hierarchical view of how home ownership impacts loan applications and disbursements.
Metrics to be shown: 'Total Loan Applications,' 'Total Funded Amount,' and 'Total Amount Received'

### Details Dashboard
GRID

Need for a comprehensive 'Details Dashboard' that provides a consolidated view of all the essential information within our loan data. This Details Dashboard aims to offer a holistic snapshot of key loan-related metrics and data points, enabling users to access critical information efficiently.

Objective: The primary objective of the Details Dashboard is to provide a comprehensive and user-friendly interface for accessing vital loan data. It will serve as a one-stop solution for users seeking detailed insights into our loan portfolio, borrower profiles, and loan performance.

## Tools
| Tools | Purpose |
| --- | --- |
| Excel | Explore, Clean, Analyze & Visualize the data |
| SQL | Testing and Analyzing the data |
| Power Bi | Visualizing the data with interactive dashboards |
| Github | Hosting the project documentation |

## Data Exploration notes
I observed that the dataset can be categorized into three sections 
   Applicant Details: id, emp_length, emp_title, annual_income, application_type, home_ownership
   Loan Details: loan_amount, term, int_rate, installment, loan_status, grade, sub_grade, purpose
   Payment and Credit History: total_payment, dti (debt-to-income), total_acc, issue_date, last_payment_date, next_payment_date, last_credit_pull_date

Excel was used to check through for null values, and emp_title field had null values.
While loading the dataset into SQL, four fields were in the wrong data type.

What steps were taken to clean and shape the data?
- emp_title field was found to be a negligible field hence nothing was done to it
- The fields with wrong data type were fixed in SQL

# Testing
SQL was used primarily for testing the data

# Visualization
## Results

This shows the Summary Dashboard

This shows the Overview Dashboard

This shows the Details Dashboard

## Measures
### Top KPIs required
### Total Loan Applications
```sql

```
### Total Funded Amount
```sql

```

### Total Received Amount
```sql

```
