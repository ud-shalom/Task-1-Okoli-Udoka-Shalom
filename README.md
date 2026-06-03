Project 1: Data Cleaning & Preparation Report
📌 Project Overview
This repository contains Project 1: Data Cleaning & Preparation, the foundation phase of the DecodeLabs Industrial Training Kit (Batch 2026). The goal of this project is to transform a raw, noisy e-commerce dataset into a reliable "source of truth" by enforcing data integrity before analytical modeling begins.

Tool Used: Excel Power Query

Core Focus: Data Integrity, Schema Standardization, and Quality Assurance

🛠️ Data Cleaning Steps (Power Query)
Data was safely loaded via From Table/Range to protect the original source file. The following transformations were applied:

Removed Duplicates: Dropped duplicate rows in OrderID to prevent artificial inflation of order counts and revenue totals.

Handled Missing Values: Replaced blank/null cells in CouponCode with "Unknown" to standardize marketing filters.

Standardized Text Case: Applied Capitalize Each Word to text columns (e.g., ReferralSource) to merge duplicate categories caused by case variations (e.g., Facebook vs facebook).

Extracting Month & Year Columns: Created two brand-new columns—Year and Month Name—directly derived from the raw Date column using text conversion formulas to break down time trends easily.

Chronological Normalization: Transformed unformatted system serial numbers (like 44930) into standard, readable date formats (YYYY-MM-DD).

Fixed Formats: Cast the Date column strictly to Date type and rounded the TotalPrice column to 2 decimal places to align with financial corporate standards.

🎯 Conclusion
The dataset was successfully exported via Close & Load. All formatting errors, duplicate records, and null values have been resolved. The data is verified, 100% clean, and fully prepared for downstream analysis and visualization.
