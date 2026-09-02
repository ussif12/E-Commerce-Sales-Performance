# 🛒 E-Commerce Sales Performance Analysis

## 📌 Project Overview
An end-to-end sales performance dashboard for an e-commerce platform, analyzing over **192.76M EGP** in total sales across **8,000 orders** and **18,000 items sold**. This project tracks key performance indicators (KPIs), consumer payment choices, regional performance, and sales category dynamics.

---

## 🎯 Business Problem
The executive team needed visibility into revenue trends, regional customer distribution, and payment method breakdown to optimize marketing budgets, regional inventory, and payment processing fees.

---

## 🛠️ Tech Stack & Tools
* **Power BI**: Built interactive dashboard layouts with slicers and dynamic category visual cards.
* **Power Query**: Data cleaning, handling null/unknown values, and standardizing category names.
* **DAX**: Created custom measures for revenue aggregations, AOV, and volume metrics.

---

## 🧹 Data Cleaning & Transformation
* Standardized city names and categorized missing locations as `Unknown`.
* Grouped transactions by payment methods and product categories.
* Created date-based aggregations to visualize monthly sales trajectory.

---

## 📐 Key DAX Measures Used
```dax
Total Sales = SUM('Sales'[Sales_Amount])
Total Orders = DISTINCTCOUNT('Sales'[Order_ID])
Average Order Value (AOV) = DIVIDE([Total Sales], [Total Orders], 0)
Total Quantity = SUM('Sales'[Quantity])
📊 Key Business MetricsTotal Sales: 192.76M EGP  Total Orders: 8,000 Orders[cite: 2]Average Order Value (AOV): 24.95K EGP[cite: 2]Total Quantity Sold: 18,000 Units[cite: 2]
💡 Key Business Insights
Top Revenue Category: Electronics drives the vast majority of revenue at 147.5M EGP, followed by Furniture at 23.34M EGP[cite: 2].

Payment Method Balance: Payment preferences are evenly split across InstaPay (49.22M EGP), Credit Cards (48.41M EGP), Vodafone Cash (47.72M EGP), and Cash on Delivery (47.4M EGP)[cite: 2].

Regional Leaders: Giza (40M EGP) and Alexandria (39M EGP) represent the top two highest-revenue regions[cite: 2].

Seasonal Trend: Sales peaked strongly in the first half of the year before stabilizing in H2[cite: 2].
🚀 Business Recommendations
Inventory Allocation: Increase stock levels for Electronics items in regional hubs like Giza and Alexandria[cite: 2].

Promotional Campaigns: Launch targeted mid-year and year-end promotional campaigns to boost sales volume during slower months[cite: 2].
