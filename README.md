# 📊 Bank Customer Churn Analysis
A comprehensive Power BI dashboard that analyzes customer churn behavior in the banking sector. This project helps stakeholders understand patterns leading to customer attrition and provides insights for improving retention strategies.

# 🧠 Problem Statement
Banking institutions face challenges in customer retention. Identifying the characteristics of customers likely to churn enables banks to proactively address issues and improve services. This project analyzes key metrics to uncover churn drivers.

# 📂 Project Overview
Tool Used: Power BI
Key Focus Areas:

# Total vs. Active vs. Inactive Customers

Credit Card vs. Non-Credit Card Holders

Monthly Churn and Retention Trends

Customer Distribution by Geography and Tenure

Impact of Features like Balance, Tenure, and Services Used on Churn

# 📈 Dashboard Insights
KPIs Tracked:
Total Customers

Active vs. Inactive Customers

Credit Card Holders

Churned Customers (Exited)

Retained Customers

Monthly Customer Trends

Churn by Geography, Gender, and Age

Tenure and Balance Analysis

# Visualizations:
Bar & Column Charts – Churn rate by demographics

Line Charts – Monthly churn and retention trends

Pie Charts – Service usage and credit card distribution

Slicers – Filter by Geography, Gender, and Credit Card status

Cards – Display key KPIs

# 📌 Features
Fully interactive slicers and filters

Drill-down capabilities for detailed view

Industry-standard report layout for executive presentation

Custom DAX measures for accurate KPIs

# 🛠️ Technical Stack
Power BI Desktop for data modeling and visualization

DAX (Data Analysis Expressions) for calculated columns and measures

Power Query (M language) for data cleaning and transformation


# 🧮 Sample DAX Measures

Exit Customers =
CALCULATE(
    COUNTROWS(CustomerData),
    CustomerData[Exited] = 1
)

Retained Customers =
CALCULATE(
    COUNTROWS(CustomerData),
    CustomerData[Exited] = 0
)

Churn Rate (%) =
DIVIDE([Exit Customers], [Total Customers]) * 100
