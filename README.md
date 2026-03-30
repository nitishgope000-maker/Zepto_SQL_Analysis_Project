🛒 Zepto SQL Data Analysis Project
🔗 Data Source & Context

This project is inspired by real-world quick-commerce operations like Zepto, focusing on product pricing, discounts, inventory, and revenue analytics.

🛒 Zepto Platform: https://www.zeptonow.com/
📊 Dataset Source (Kaggle): https://www.kaggle.com/your-dataset-link

📌 Note: This dataset is sourced from Kaggle and used for educational and analytical purposes only.

📌 Project Overview

This project focuses on analyzing product-level data from an e-commerce platform using SQL. The goal is to extract actionable business insights related to pricing strategies, discount patterns, inventory distribution, and revenue estimation.

The analysis is performed entirely using SQL, simulating real-world business problem-solving scenarios.

🎯 Objectives
Perform data exploration and cleaning
Analyze pricing and discount strategies
Generate business insights for decision-making
Understand inventory and stock distribution
Evaluate revenue potential across categories
🗂️ Dataset Description

The dataset consists of a structured table named zepto with the following schema:

Column Name	Description
sku_id	Unique product identifier
category	Product category
name	Product name
mrp	Maximum Retail Price (₹)
discountPercent	Discount percentage
availableQuantity	Available stock
discountedSellingPrice	Selling price after discount
weightInGms	Product weight (grams)
outOfStock	Stock availability (TRUE/FALSE)
quantity	Quantity per unit
🧹 Data Cleaning Steps
Removed products with invalid pricing (MRP = 0)
Converted price values from paise to rupees
Checked and handled NULL values
Identified duplicate product entries
Standardized numerical formats for analysis
🔍 Data Exploration
Total number of products in dataset
Unique product categories
Stock availability distribution (in-stock vs out-of-stock)
Duplicate product detection
📊 Key Business Insights
1️⃣ Top Discounted Products

Identified products offering the highest discount percentages.

2️⃣ High-Value Out-of-Stock Products

Analyzed expensive products (MRP > ₹300) that are currently unavailable.

3️⃣ Category-wise Revenue Estimation

Estimated revenue using:

SUM(discountedSellingPrice * availableQuantity)
4️⃣ Premium Low-Discount Products

Filtered products with:

MRP > ₹500
Discount < 10%
5️⃣ Best Discount Categories

Top 5 categories offering the highest average discounts.

6️⃣ Price Efficiency Analysis

Calculated price per gram to identify best-value products.

7️⃣ Product Segmentation

Segmented products into:

Low weight (< 1kg)
Medium weight (1kg–5kg)
Bulk (> 5kg)
8️⃣ Inventory Weight Analysis

Computed total inventory weight per category.

🧠 Key Learnings
Writing advanced SQL queries using:
GROUP BY
HAVING
CASE WHEN
Aggregate functions
Performing real-world data cleaning
Translating raw data into business insights
Understanding e-commerce analytics workflows
🛠️ Tech Stack
SQL (MySQL / PostgreSQL)
MySQL Workbench / pgAdmin
🚀 How to Run This Project
Create a new database
Import the SQL file
Run queries step-by-step
SOURCE zepto_project.sql;
📈 Future Improvements
Build an interactive Power BI / Tableau dashboard
Perform time-series analysis
Use Python (Pandas) for deeper insights
Add predictive analytics / ML models
🤝 Connect With Me
💼 LinkedIn: https://www.linkedin.com/in/your-profile
⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub!
