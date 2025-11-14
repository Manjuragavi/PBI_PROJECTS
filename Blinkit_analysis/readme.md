# 📊 Blinkit Sales & Performance Analysis – Power BI Dashboard

## 📘 Project Overview
This Power BI project presents an in-depth analysis of Blinkit's sales, customer behavior, and operational performance.  
The dashboard provides interactive insights that help stakeholders make data-driven decisions with ease.

---

## 🎯 Objectives
- Analyze total sales, revenue trends, and growth patterns.
- Understand customer segments and order behavior.
- Evaluate product/category performance.
- Assess operational metrics like delivery time and cancellations.
- Build a visually dynamic and decision-oriented Power BI dashboard.

---

## 🛠️ Tools & Technologies
- **Power BI Desktop**
- **Power Query**
- **DAX (Data Analysis Expressions)**
- **Data Modelling (Star Schema)**
- **Excel / CSV Data Sources**

---

## 📂 Dataset Details
Dataset consists of:
- Order ID  
- Order Date  
- Customer ID  
- Product Name  
- Category  
- Selling Price  
- Quantity  
- Revenue  
- Delivery Time  
- Customer Rating  
- Location / Outlet Information  

---

## 📐 Key Features of the Dashboard

### **1️⃣ Sales Overview**
- Total Revenue
- Total Orders
- Average Order Value (AOV)
- Monthly & Daily Sales Trends
- Category-wise Revenue

### **2️⃣ Customer Insights**
- New vs Returning Customers
- Customer Ratings Trend
- Top Customer Locations

### **3️⃣ Product & Category Analysis**
- Best-selling Products
- Category Contribution
- Price vs Quantity Patterns

### **4️⃣ Operational Metrics**
- Delivery Time Distribution
- Cancellation Rate
- Fulfillment Performance
- Inventory/Stock Indicators

---

## 🧠 DAX Measures Used
```DAX
Total Revenue = SUM(Sales[Revenue])

Total Orders = DISTINCTCOUNT(Sales[Order ID])

AOV = [Total Revenue] / [Total Orders]

Total Quantity = SUM(Sales[Quantity])

Monthly Revenue = 
CALCULATE(
    [Total Revenue],
    GROUPBY(Sales, Sales[Order Date].[Month])
)

---
## 🚀 Key Insights

✔ **Sales Trends**
- Revenue peaks during weekends and promotional periods.
- Category "Groceries" and "Dairy" contribute the highest sales share.

✔ **Customer Behavior**
- Returning customers generate ~40% more revenue than new customers.
- Ratings remain consistent, indicating strong customer satisfaction.

✔ **Product Performance**
- Top 10 items contribute nearly 60% of total revenue.
- Certain low-priced items sell in high quantities, boosting volume-based revenue.

✔ **Operational Insights**
- Average delivery time is within the expected SLA range.
- A few cities face slightly higher delays, needing operational improvement.

---

## 📌 Conclusion

The Blinkit Power BI Dashboard provides a clear, data-driven view of the company’s business performance.  
From sales patterns to customer behavior and delivery operations, this dashboard brings all critical insights into one place.

It helps decision-makers:
- Identify growth opportunities  
- Improve fulfillment efficiency  
- Understand customer needs  
- Optimize product strategies  

Overall, this project showcases effective data modelling, DAX calculations, and visualization expertise using Power BI.



