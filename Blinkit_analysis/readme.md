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

