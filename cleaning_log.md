# Cleaning Log

## Project
Business Analytics Assignment - Order Dataset Cleaning

**Dataset:** raw_orders.xlsx

---

# 1. Issues Found

The following data quality issues were identified in the raw dataset:

- Multiple date formats in Order Date and Ship Date columns.
- Leading and trailing spaces in text columns.
- Inconsistent capitalization in Ship Mode and other text fields.
- Missing values in Discount and Ship Mode.
- Invalid discount values (negative values and values greater than 50%).
- Sales, Cost and Profit validation mismatches.
- Duplicate record check performed.
- Order status and payment status inconsistencies.

---

# 2. Cleaning Actions Performed

The following cleaning actions were completed:

- Standardized all Order Date values to YYYY-MM-DD format.
- Standardized all Ship Date values to YYYY-MM-DD format.
- Removed extra spaces from text columns.
- Standardized Region names.
- Standardized Segment names.
- Standardized Customer Names.
- Standardized Ship Mode values.
- Cleaned Discount values.
- Filled missing Ship Mode values where applicable.
- Created calculated columns.
- Validated Sales and Profit calculations.
- Checked duplicate records.
- Generated Data Quality Report.
- Generated Pivot Summary Report.

---

# 3. Business Rules Applied

The following business rules were applied during cleaning:

- Discount cannot be negative.
- Discount cannot exceed 50%.
- Ship Date cannot be earlier than Order Date.
- Sales = Quantity × Unit Price × (1 − Discount)
- Profit = Sales − Cost
- Missing text values were standardized.
- Invalid records were flagged instead of deleted whenever possible.

---

# 4. Assumptions Made

- Missing discounts were treated as 0 where appropriate.
- Text formatting differences were considered formatting issues.
- Invalid discount values were corrected according to business rules.
- Date values were converted into ISO format (YYYY-MM-DD).
- Minor spacing and capitalization differences were standardized.

---

# 5. Records Removed

No records were permanently deleted.

Duplicate check completed.

Duplicate records removed: 0

---

# 6. Records Flagged

Records were flagged for:

- Missing values
- Invalid discount
- Date inconsistency
- Status mismatch
- Calculation mismatch

Data Quality Flag values used:

- CLEAN
- WARNING
- INVALID

---

# 7. Calculated Columns Created

The following calculated columns were added:

- cleaned_discount
- calculated_sales
- calculated_profit
- profit_margin
- shipping_delay_days
- order_month
- order_year
- data_quality_flag

---

# 8. Validation Performed

Validation checks included:

- Missing value analysis
- Duplicate analysis
- Date validation
- Discount validation
- Text cleaning validation
- Sales calculation validation
- Profit calculation validation
- Business rule validation

---

# 9. Output Files Generated

- cleaned_orders.xlsx
- data_quality_report.xlsx
- pivot_summary.xlsx
- cleaning_log.md
- README.md

---

# 10. Limitations

- Cleaning decisions were based on the provided business rules.
- Missing values were handled using standard assumptions.
- No external reference data was used.
- Business calculations were validated using available dataset values.

---

# Cleaning Completed Successfully