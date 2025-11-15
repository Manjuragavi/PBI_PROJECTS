# 📊 Bank Customer Analysis | Power BI Project

A comprehensive Power BI solution designed to analyze customer demographics, financial behavior, and engagement patterns within a banking ecosystem. This project delivers actionable insights that empower strategic decision-making in customer segmentation, product optimization, and operational efficiency.

---

## 📁 Project Overview

The **Bank Customer Analysis Dashboard** highlights key behavioral and financial trends among customers. It leverages interactive visualizations to uncover patterns in customer demographics, account balance distribution, credit utilization, and churn-related indicators.

This project demonstrates strong BI capabilities including data modeling, DAX measures, data cleaning, KPI tracking, and advanced visualization techniques.

---

## 🎯 Objectives

- Understand customer demographics and financial behavior  
- Identify high-value customers and risk-prone categories  
- Track account performance and product utilization  
- Support data-driven decision-making for customer retention and service improvement

---

## 🛠️ Tech Stack

- **Power BI Desktop**
- **Power Query**
- **DAX (Data Analysis Expressions)**
- **Excel / CSV Data Sources**

---
## Dashboard Visualization
<img width="1062" height="606" alt="Bank analysis Dashboard Image" src="https://github.com/user-attachments/assets/67f41189-0218-468d-9d86-624616e6589d" />

## Dashboard Insights
### 1. Customer Activity Chart
   This chart represents the proportion of active and inactive customers. It visually highlights how customer engagement levels vary within the bank.
### 2. Monthly Trend Chart
   The trend chart shows how customer behavior changes month by month. It helps in identifying specific months with higher or lower activity or exits, giving insights into seasonal or operational factors.
### 3. Gender Distribution Chart
   This chart illustrates the distribution of customers based on gender. It helps to understand the balance between male and female customers and how their engagement levels differ.
### 4. Credit Score Category Chart
   This visualization represents customers grouped by their credit score levels such as “Good,” “Very Good,” and “Excellent.” It helps the bank identify which credit groups are more likely to remain active or inactive.
### 5. Summary Cards
   The dashboard includes cards that provide a quick overview of total customers, active/inactive members, and credit card users. These cards make it easy to view the bank’s key statistics at a glance.

   -----
## DAX Formulas Used
- Max_Credit = MAX(Bank[CreditScore])
- Totalcustomer = COUNT(Bank[CustomerId])
- Active Member = CALCULATE(COUNT(Bank[IsActiveMember]),KEEPFILTERS(Bank[IsActiveMember]=1))
- Inactive Member = CALCULATE(COUNT(Bank[IsActiveMember]),KEEPFILTERS(Bank[IsActiveMember]=0))
- Credit Holder = CALCULATE(COUNT(Bank[HasCrCard]),KEEPFILTERS(Bank[HasCrCard]=1))
- Not Credit Holder = CALCULATE(COUNT(Bank[HasCrCard]),KEEPFILTERS(Bank[HasCrCard]=0))
- Retain Customers = CALCULATE(COUNT(Bank[Exited]),KEEPFILTERS(Bank[Exited]=0))
- Exit Customers = CALCULATE(COUNT(Bank[Exited]),KEEPFILTERS(Bank[Exited]=1))

  ------
## Conclusion
The project highlights how visual analytics can help the bank better understand its customers and make data-driven decisions.
To improve business outcomes based on this analysis:
- Increase engagement programs to encourage inactive customers.
- Focus on improving service experience to retain customers with good credit profiles.
- Conduct periodic feedback surveys to identify satisfaction levels and areas needing attention.
- Strengthen personalized offers and communication to build long-term relationships.
#### These improvements will help the bank enhance customer satisfaction, reduce customer exits, and build stronger customer loyalty over time.



