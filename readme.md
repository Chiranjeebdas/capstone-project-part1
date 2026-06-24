# Business Analytics Capstone Project – Part 1
## Data Cleaning and Quality Assessment

---

## Project Overview

This project focuses on cleaning and preparing an order dataset for business analysis. The raw dataset contained inconsistent date formats, missing values, invalid discounts, inconsistent text formatting, and business rule violations. The dataset was cleaned, validated, and transformed into an analysis-ready format.

---

## Objectives

- Improve overall data quality.
- Standardize text and date formats.
- Validate business rules.
- Generate calculated business metrics.
- Create pivot summaries for business insights.
- Prepare a clean dataset for further analytics.

---

## Dataset Information

**Dataset Name:** raw_orders.xlsx

**Records:** 932

**Columns:** 21

---

## Folder Structure

```
business_analytics_assignment/
│
├── data/
│   └── raw_orders.xlsx
│
├── outputs/
│   ├── cleaned_orders.xlsx
│   ├── data_quality_report.xlsx
│   ├── pivot_summary.xlsx
│   └── cleaning_log.md
│
├── screenshots/
│   ├── raw_data_preview.png
│   ├── cleaned_data_preview.png
│   ├── data_quality_report.png
│   ├── pivot_summary_1.png
│   ├── pivot_summary_2.png
│   └── pivot_summary_3.png
│
└── README.md
```

---

# Data Cleaning Performed

The following cleaning operations were completed:

- Standardized Customer Names.
- Standardized Segment values.
- Standardized Region values.
- Standardized State values.
- Standardized City values.
- Standardized Category values.
- Standardized Sub-Category values.
- Standardized Ship Mode values.
- Standardized Payment Status.
- Standardized Order Status.
- Converted Order Date into YYYY-MM-DD format.
- Converted Ship Date into YYYY-MM-DD format.
- Removed leading and trailing spaces.
- Corrected inconsistent text capitalization.
- Cleaned invalid discount values.
- Validated missing values.
- Checked duplicate records.

---

# Calculated Columns

The following calculated columns were created:

- cleaned_discount
- calculated_sales
- calculated_profit
- profit_margin
- shipping_delay_days
- order_month
- order_year
- data_quality_flag

---

# Business Rules Applied

The following business rules were validated:

- Discount cannot be negative.
- Discount cannot exceed the allowed limit.
- Ship Date cannot be earlier than Order Date.
- Sales = Quantity × Unit Price × (1 − Discount)
- Profit = Sales − Cost
- Profit Margin = Profit ÷ Sales

---

# Data Quality Checks

The dataset was validated for:

- Missing values
- Duplicate records
- Invalid discounts
- Invalid shipping dates
- Text consistency
- Date consistency
- Business rule validation

---

# Pivot Analysis

Three Pivot Tables were created:

1. Sales by Region
2. Category Performance
3. Monthly Sales Trend

---

# Files Included

- raw_orders.xlsx
- cleaned_orders.xlsx
- data_quality_report.xlsx
- pivot_summary.xlsx
- cleaning_log.md
- README.md

---

# Tools Used

- WPS Office Spreadsheet
- Microsoft Excel Functions
- Pivot Tables
- Data Validation

---

# Project Outcome

The final cleaned dataset is ready for business analysis and reporting. Data quality issues were identified, corrected, and documented. The generated reports and pivot summaries provide valuable business insights for decision-making.

---

# Author

**Name:** Chiranjeeb Das

Business Analytics Capstone Project
