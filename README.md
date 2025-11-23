# Customer-Churn-Analysis

Customer Churn Analysis – Python, SQL & Data Visualization

This project analyzes customer churn behavior using Python, SQL-style queries, and visualizations. The goal is to understand why customers leave, identify the key churn drivers, and generate actionable insights to help improve retention.

🛠 Tools & Skills Used

Python: Pandas, NumPy, Seaborn, Matplotlib

SQL (via pandasql): Aggregations, filtering, grouping

Visualization: Countplots, bar charts, heatmaps

EDA: Statistical exploration, feature understanding

Dataset Overview

The dataset includes the following fields:

CustomerID

Age

Gender

Subscription Type (Basic / Standard / Premium)

Contract Length (Monthly / Quarterly / Yearly)

Usage Frequency

Support Calls

Payment Delay

Total Spend

Last Interaction

Churn (0/1)

Total Rows: 64,374
Target Variable: Churn

Data Cleaning Steps

Converted Churn column to integer

Created AgeGroup for better segmentation

Verified no missing values in main fields

Ensured numerical and categorical formats were correct

Removed duplicates

Exploratory Data Analysis (Python)
✔ 1. Churn Distribution

Shows how many customers churned vs stayed.

✔ 2. Churn by Contract Length

Monthly contracts had the highest churn
Quarterly and Yearly customers churned less.

✔ 3. Churn by Subscription Type

Basic users churn the most

Premium users churn the least — strongest loyalty segment

✔ 4. Churn by Age Group

Younger customers (18–25) and mid-range (46–55) churn more.

✔ 5. Correlation Heatmap

Key findings from heatmap:

Payment Delay → Strong positive correlation with Churn

Support Calls → Strong positive correlation with Churn

Usage Frequency → Negative correlation with Churn

Total Spend → Negative correlation with Churn

🧮 SQL Queries (Executed with pandasql)

SQL was applied directly to the dataframe using pandasql.

1️⃣ Churn Count by Subscription Type
2️⃣ Average Payment Delay by Churn
3️⃣ Contract Length vs Churn
4️⃣ High-Risk Customer Segment

Key Insights

Payment Delay is the strongest churn driver — customers with frequent delays churn significantly more.

More Support Calls = Higher Churn — indicates dissatisfaction or recurring issues.

Monthly Contract customers churn the most; Yearly plans retain customers better.

Basic plan users churn more while Premium users have the lowest churn rate.

Higher Usage Frequency reduces churn, showing engagement leads to retention.

Higher Total Spend correlates with lower churn — loyal, high-value customers stay longer.
