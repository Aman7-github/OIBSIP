# Task 2 — Customer Segmentation Analysis

## Objective
Apply clustering algorithms to segment an e-commerce company's customer base into distinct groups based on 
purchasing behaviour, enabling targeted marketing strategies.

## Tech Stack
Python, pandas, scikit-learn (KMeans), matplotlib, seaborn, Jupyter Notebook

## Approach
- Calculated RFM (Recency, Frequency, Monetary) features per customer
- Standardized features using StandardScaler
- Applied K-Means clustering (K=4, selected via Elbow Method)
- Visualized clusters using scatter plots (Recency vs Monetary, Frequency vs Monetary)
- Profiled each cluster's average Recency, Frequency, and Monetary values

## Key Findings
- **Cluster 0 — Recent, Low Spenders:** Shopped recently but spend the least (40,618 customers)
- **Cluster 1 — Big Spenders:** Highest spenders by far, smallest group (4,015 customers)
- **Cluster 2 — Inactive, Low Spenders:** Long time since last purchase, low spend (40,531 customers)
- **Cluster 3 — Mid Spenders:** Moderate spend and recency (14,293 customers)

## Marketing Recommendations
- **Recent Low Spenders:** Upsell/cross-sell offers
- **Big Spenders:** VIP loyalty rewards and early access
- **Inactive Customers:** Win-back campaigns
- **Mid Spenders:** Targeted promotions to move them toward higher-value segment

## Output
Full analysis, charts, and cluster profiles documented in the notebook.