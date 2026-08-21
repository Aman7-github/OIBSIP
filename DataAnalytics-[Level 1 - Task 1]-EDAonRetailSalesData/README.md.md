# Task 1 — Exploratory Data Analysis on Retail Sales Data

## Objective
Perform exploratory data analysis (EDA) on an e-commerce retail sales dataset to uncover customer 
demographics, purchasing patterns, and revenue drivers across categories, payment methods, and locations.

## Tech Stack
Python, pandas, numpy, matplotlib, seaborn, Jupyter Notebook

## Dataset
E-commerce customer shopping dataset (99,457 rows, 10 columns) — invoice details, customer demographics 
(gender, age), product category, quantity, price, payment method, purchase date, and shopping mall.

## What This Notebook Covers
- Data loading, structure inspection, and missing value check (no missing values found)
- Feature engineering: added `month`, `year`, `total_sales`, and `age_group` columns
- Gender breakdown of customers
- Category-wise purchase % and sales analysis
- Age-group-wise customer distribution
- Payment method distribution analysis
- Top 10 shopping malls by sales

## Key Insights

**Category-wise Purchase %**
Clothing has the highest purchase share (45.33%), followed by Electronics and Home & Kitchen — customers are 
more inclined to spend on clothing and accessories than other categories.

**Category-wise Sales**
Clothing is the top category by total sales (114.00M); Souvenir is the lowest (0.64M).

**Customer Age Group**
The 56+ age group has the highest customer count (26,587 customers, 26.73% of the base) — the largest segment. 
The 18-25 age group is the least represented, at only 15.44%.

**Payment Method**
Cash is the most used payment method by purchase volume (112.83M, 44.86% share) — the least used payment 
method has a smaller share.

**Shopping Malls**
Mall of Istanbul generates the highest sales (50.87M, 20.23% market contribution). Forum Istanbul has the 
lowest sales among the top 10 malls (12.30M, 4.89% contribution).

## Conclusion & Recommendations

1. **Age doesn't affect spending** — Since age showed no link to purchase behavior, marketing doesn't need to 
   target specific age groups; focus budget elsewhere instead.
2. **Cash is the most-used payment method; Debit Card is the least** — This is worth investigating further; 
   the business could consider incentives (e.g. discounts) to encourage more card usage, though this would 
   need testing since discount impact isn't part of this dataset.
3. **Female customers outnumber male customers in every age group** — A campaign or product mix aimed at male 
   shoppers could help grow this underrepresented segment.

## Output
Full analysis, charts, and written insight sections documented directly in the notebook.