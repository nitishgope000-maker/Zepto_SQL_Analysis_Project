🛒 Zepto SQL Data Analysis Project
📌 Project Overview

This project focuses on analyzing product-level data from an e-commerce platform (Zepto) using SQL. The goal is to extract actionable business insights related to pricing, discounts, inventory, and revenue.

The dataset includes product attributes such as category, pricing, discounts, stock availability, and weight.

🎯 Objectives
Perform data exploration and cleaning
Analyze pricing and discount strategies
Generate business insights for decision-making
Optimize understanding of inventory and revenue patterns
🗂️ Dataset Description

The dataset consists of a structured table named zepto with the following schema:

Column Name	Description
sku_id	Unique product identifier
category	Product category
name	Product name
mrp	Maximum Retail Price
discountPercent	Discount percentage
availableQuantity	Available stock
discountedSellingPrice	Selling price after discount
weightInGms	Product weight
outOfStock	Stock status
quantity	Quantity per unit
🧹 Data Cleaning Steps
Removed products with invalid pricing (MRP = 0)
Converted price values from paise to rupees
Checked and handled NULL values
Verified duplicate product entries
🔍 Data Exploration
Total number of records
Unique product categories
Stock availability distribution
Duplicate product identification
📊 Key Business Insights
1️⃣ Top Discounted Products
Identified products with the highest discount percentages
2️⃣ High-Value Out-of-Stock Products
Found expensive products (MRP > ₹300) that are unavailable
3️⃣ Category-wise Revenue Estimation
Calculated total revenue using:
SUM(discountedSellingPrice * availableQuantity)
4️⃣ Premium Low-Discount Products
Products with:
MRP > ₹500
Discount < 10%
5️⃣ Best Discount Categories
Top 5 categories offering highest average discounts
6️⃣ Price Efficiency Analysis
Computed price per gram to identify best-value products
7️⃣ Product Segmentation
Categorized products into:
Low weight
Medium weight
Bulk
8️⃣ Inventory Weight Analysis
Total inventory weight per category
🧠 Key Learnings
Writing complex SQL queries using:
GROUP BY
CASE WHEN
HAVING
Aggregate functions
Real-world data cleaning techniques
Translating raw data into business insights
Understanding e-commerce analytics use cases
🛠️ Tech Stack
SQL (MySQL / PostgreSQL compatible)
Database Tools:
MySQL Workbench
pgAdmin
🚀 How to Run This Project
Create a database

Run the SQL script:

SOURCE zepto_project.sql;
Execute queries step-by-step for analysis
📈 Future Improvements
Build a Power BI / Tableau dashboard
Add time-series sales analysis
Integrate Python (Pandas) for advanced analytics
Perform customer segmentation
🤝 Connect With Me

If you like this project, feel free to connect and collaborate!

💼 LinkedIn: (https://www.linkedin.com/in/nitish-gope-58370a236/)


If you found this project useful, consider giving it a ⭐ on GitHub!
