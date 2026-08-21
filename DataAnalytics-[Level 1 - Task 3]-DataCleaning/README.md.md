# Task 3 — Data Cleaning Project

## Objective
Take a deliberately messy dataset and systematically transform it into a clean, analysis-ready dataset, 
documenting every decision — demonstrating professional-level data cleaning skills.

## Tech Stack
Python, pandas, numpy, Jupyter Notebook

## Dataset
Synthetic e-commerce customer dataset (11,056 rows, 11 columns) with deliberately injected issues: missing 
values, duplicate rows, inconsistent text formatting, mixed date formats, currency symbols, invalid values, 
and outliers.

## Cleaning Process
| Column | Issues Found | Action Taken |
|---|---|---|
| Age | Invalid values (-5, 0, 999), missing | Treated invalid as missing, filled with median |
| Gender | Inconsistent casing/spacing, high missing rate | Standardized, filled with mode |
| City | Inconsistent casing, naming variants | Standardized, merged variants, filled with mode |
| Category | Minor casing issues | Standardized, filled with "Unknown" |
| Quantity | Text entries, negative/zero values | Converted to numeric, filled with median |
| Price | Currency symbols, negatives, extreme outliers | Cleaned, capped outliers (IQR method), filled with median |
| PaymentMethod | Abbreviations, casing inconsistencies | Standardized to consistent labels |
| PurchaseDate | Mixed formats, invalid placeholder dates | Parsed flexibly, left unparseable as missing |
| CustomerID/Name/Email | Missing identifiers | Rows dropped (can't be imputed) |
| Duplicates | 555 exact duplicate rows | Removed |

## Key Design Decisions
- Used median for numeric imputation (robust to outliers)
- Used mode for categorical columns with a clear typical value
- Used "Unknown" instead of guessing where fabricating a value could distort analysis
- Capped (not removed) price outliers to preserve row count
- Dropped rows missing unique identifiers

## Output
Cleaned dataset saved as `customer_data_cleaned.csv`.