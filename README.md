# Customer Segmentation using RFM Analysis

## Project Objective

This project aims to perform a customer segmentation analysis on a transactional dataset from an online retailer. By applying the RFM (Recency, Frequency, Monetary) model, the goal is to group customers into distinct segments and provide strategic recommendations for targeted marketing campaigns.


---

## Skills Demonstrated

* **Advanced Data Cleaning:** Python (Pandas) for handling missing values, returns, and data type conversions.
* **Data Transformation:** Complex data aggregation and feature engineering using `groupby()` and `agg()` to calculate RFM metrics.
* **Statistical Analysis:** Application of quantiles (`pd.qcut`) for customer scoring.
* **Data Visualization:** Python (Matplotlib & Seaborn) for visualizing segment distribution.
* **Business Strategy:** Translating data-driven segments into actionable marketing recommendations.

---

## Key Findings & Recommendations

The analysis successfully grouped customers into seven distinct segments, revealing the following insights:

1.  **High-Value Segments (`Champions`, `Potential Loyalists`):** A significant portion of the customer base consists of our most valuable customers.
    * **Recommendation:** Nurture these segments with loyalty programs and exclusive access to new products to maximize retention.

2.  **At-Risk Customers:** A smaller but highly valuable group of customers who used to be active but have not purchased recently.
    * **Recommendation:** Launch a targeted "win-back" campaign with personalized offers to re-engage them before they churn.

3.  **New Customers:** A healthy number of new customers have made recent purchases but have not yet become frequent buyers.
    * **Recommendation:** Focus on onboarding and encouraging a second purchase through a follow-up discount or product recommendations.

---

## Process

1.  **Data Cleaning:** Loaded a raw transactional dataset, removed rows with missing `CustomerID`, filtered out returned orders, and handled data type issues.
2.  **Feature Engineering:** Calculated a `TotalPrice` column for each transaction.
3.  **RFM Calculation:** Aggregated the transactional data to calculate Recency, Frequency, and Monetary values for each unique customer.
4.  **Scoring & Segmentation:** Scored each customer from 1-5 on each RFM metric using quintiles. Combined these scores to group customers into strategic segments like "Champions," "At-Risk," and "New Customers."
5.  **Analysis & Visualization:** Summarized the segments and visualized the distribution of customers using a bar chart.
