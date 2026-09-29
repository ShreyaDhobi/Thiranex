# Data Cleaning & Reporting Automation

## Project Overview

This project focuses on automating data cleaning and reporting workflows using Python and historical retail transaction data.

The raw retail data is processed to handle missing values, duplicate records, and inconsistent transaction values. After cleaning the data, an automated summary report and visual summary are generated to make the data easier to understand and analyze.

## Objectives

- Clean and preprocess the retail transaction data.
- Handle missing values and duplicate records.
- Identify and remove inconsistent transaction values.
- Generate an automated summary report.
- Create visual summaries from the cleaned data.

## Dataset

The project uses the Online Retail II Dataset, which contains historical retail transaction data from 2009 to 2011.

The dataset includes information such as:

- Invoice
- StockCode
- Description
- Quantity
- InvoiceDate
- Price
- Customer ID
- Country

## Data Cleaning

The following data cleaning steps are performed:

- Inspecting the dataset for missing values.
- Removing records containing missing values.
- Identifying and removing duplicate records.
- Removing transactions with zero or negative quantities.
- Removing transactions with zero or negative prices.

These steps help prepare the dataset for accurate reporting and analysis.

## Automated Reporting

After cleaning the data, an automated summary report is generated using Python.

The report includes:

| Metric | Description |
|---|---|
| Total Transactions | Total number of cleaned transaction records |
| Total Customers | Number of unique customers |
| Total Sales | Total sales generated from the cleaned data |
| Average Transaction Value | Average sales value per transaction |

## Visual Summary

A Top 10 Countries by Sales bar chart is generated to provide a visual summary of sales distribution across different countries.

This makes it easier to identify the countries contributing the highest sales.

## Workflow

Retail Transaction Data
        ↓
Data Inspection
        ↓
Data Cleaning
        ↓
Data Validation
        ↓
Automated Report
        ↓
Visual Summary

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Project Structure

Task-4-Data-Cleaning-Reporting/
│
├── Data_Cleaning_Reporting_Automation.ipynb
└── README.md

## Key Outcomes

This project provides practical experience in:

- Data cleaning and preprocessing
- Missing value handling
- Duplicate removal
- Inconsistent data handling
- Automated report generation
- Data visualization
- Reporting workflow automation

