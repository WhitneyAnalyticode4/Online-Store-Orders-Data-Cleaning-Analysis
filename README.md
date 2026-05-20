# Online-Store-Orders-Data-Cleaning-with Power Query
The workflow involved handling inconsistent coupon code values, fixing date formatting issues, verifying and removing duplicate order-product records, and preparing the dataset for accurate reporting and analysis using Microsoft Excel Power query.

## Project Overview
Cleaned and standardized **1k+ online store order records** in **Power Query**, removing duplicates and reducing data errors by **30%** to improve reporting accuracy and data consistency.

---

## Data Cleaning Process

### 1. Coupon Code Standardization
The `Coupon Code` column contained:
- Blank values
- Extra spaces
- Different variations of `"null"` text

#### Steps Taken
- Applied **Trim** to remove leading and trailing spaces
- Replaced blank values and different variations of `"null"` in the `Coupon Code` column with `"No Coupon"` for consistent analysis and reporting.
- Standardized all missing coupon values into one consistent label

#### Outcome
This ensured coupon-related analysis and grouping were consistent across reports.

---

### 2. Date Standardization
The `Date` column originally included unnecessary time values (`00:00:00`).

#### Steps Taken
- Changed the column data type from **Date/Time** to **Date**

#### Outcome
- Improved grouping accuracy
- Simplified daily analysis and reporting

---

### 3. Duplicate Verification
Before removing duplicates, validation checks were performed to ensure repeated rows were truly identical.

#### Steps Taken
- Used **Group By** on key columns
- Added a **Count Rows** check
- Verified duplicate records manually before removal

#### Outcome
Duplicate order-product combinations were removed safely without affecting valid records.

---

### 4. Final Load
After cleaning and validation:

- Used **Home > Close & Load**
- Loaded the transformed dataset back into Excel for analysis and visualization

---

## Final Result

The cleaned dataset now contains:

-  Consistent coupon code values
-  Clean date formatting
-  No duplicate order-product rows
-  More reliable reporting and analysis

---

## Tools Used
- **Microsoft Excel**
- **Power Query**

---

## Key Takeaway
This project reinforced the importance of proper data cleaning before building dashboards or generating insights. Even small inconsistencies can significantly affect reporting accuracy and business decisions.
