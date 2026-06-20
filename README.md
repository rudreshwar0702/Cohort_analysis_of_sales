# Cohort_analysis_of_sales
Customer Churn Cohort Analysis
Project Overview

This project performs a Tenure-Based Cohort Analysis on a customer churn dataset to identify patterns in customer retention, spending behavior, service usage, and churn rates. Since the dataset does not contain transaction or signup dates, customer cohorts are created using the Tenure variable.

The analysis helps businesses understand which customer groups are more likely to churn and provides actionable insights to improve customer retention.

Dataset Information

The dataset contains 440,832 customer records with the following features:

Column Name	Description
CustomerID	Unique customer identifier
Age	Customer age
Gender	Customer gender
Tenure	Duration of customer relationship
Usage Frequency	Frequency of service usage
Support Calls	Number of customer support calls
Payment Delay	Payment delay duration
Subscription Type	Customer subscription plan
Contract Length	Length of customer contract
Total Spend	Total amount spent by customer
Last Interaction	Days since last interaction
Churn	Target variable (0 = Retained, 1 = Churned)
Objective

The primary objectives of this project are:

Analyze customer churn across different tenure groups.
Identify high-risk customer segments.
Examine relationships between usage, spending, support calls, and churn.
Generate actionable business recommendations to improve customer retention.
Methodology
1. Data Preparation
Load the dataset using Pandas.
Verify data quality and handle missing values if necessary.
Create tenure-based customer cohorts.
2. Cohort Creation

Customers are grouped into the following tenure cohorts:

Cohort	Tenure Range
0–6 M	New Customers
7–12 M	Early Customers
13–24 M	Growing Customers
25–36 M	Established Customers
37–48 M	Loyal Customers
48+ M	Long-Term Customers
3. Cohort Metrics

The following metrics are calculated for each cohort:

Customer Count
Average Total Spend
Average Usage Frequency
Average Support Calls
Churn Rate
4. Visualization

The project generates:

Churn Rate Bar Chart
Cohort Analysis Heatmap
Customer Segment Comparison
Key Insights

Typical findings may include:

High Churn Among New Customers

Customers with shorter tenure tend to exhibit higher churn rates, indicating onboarding challenges.

Loyal Customers Generate More Revenue

Long-term customers generally contribute higher spending and demonstrate lower churn rates.

Support Calls Correlate with Churn

Customers requiring frequent support are more likely to leave the service.

Usage Frequency Improves Retention

Customers who engage more frequently with the service show stronger retention behavior.

Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Project Structure
Customer-Churn-Cohort-Analysis/
│
├── data/
│   └── customer_churn.csv
│
├── notebooks/
│   └── Cohort_Analysis.ipynb
│
├── outputs/
│   ├── churn_rate_chart.png
│   └── cohort_heatmap.png
│
├── README.md
│
└── requirements.txt
How to Run
Install dependencies:
pip install pandas numpy matplotlib seaborn
Place the dataset in the project folder.
Run the Python script or Jupyter Notebook:
python cohort_analysis.py

or

jupyter notebook
View the generated charts and insights.
Business Value

This analysis enables organizations to:

Reduce customer churn.
Improve customer satisfaction.
Increase customer lifetime value.
Develop targeted retention strategies.
Identify high-risk customer segments early.
Conclusion

The Tenure-Based Cohort Analysis provides a clear understanding of customer behavior across different lifecycle stages. By identifying churn patterns and engagement trends, businesses can implement data-driven strategies to improve retention, customer satisfaction, and long-term profitability.
