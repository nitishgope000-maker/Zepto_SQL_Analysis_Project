# 🛒 Zepto SQL Data Analysis Project

## 🔗 Data Source & Context

This project is inspired by real-world quick-commerce operations like [Zepto](https://www.zeptonow.com/), focusing on product pricing, discounts, inventory, and revenue analytics.

- 🛒 Zepto Platform: https://www.zeptonow.com/
- 📊 Dataset Source (Kaggle): [Dataset](https://www.kaggle.com/datasets/palvinder2006/zepto-inventory-dataset)
> 📌 Note: This dataset is used for educational and analytical purposes only.

---

## 📌 Project Overview

This project analyzes product-level e-commerce data using SQL to extract meaningful business insights.

Key focus areas:
- Pricing strategy  
- Discount analysis  
- Inventory distribution  
- Revenue estimation  

---

## 🎯 Objectives

- Perform data exploration and cleaning  
- Analyze pricing and discount strategies  
- Generate business insights  
- Understand inventory distribution  
- Evaluate revenue potential  

---

## 🗂️ Dataset Description

The dataset contains a table named `zepto` with the following columns:

| Column Name | Description |
|------------|------------|
| sku_id | Unique product ID (Synthetic Primary Key)|
| category | Product category |
| name | Product name |
| mrp | Maximum Retail Price (₹) |
| discountPercent | Discount % |
| availableQuantity | Units available in stock|
| discountedSellingPrice | Selling price |
| weightInGms | Weight in grams |
| outOfStock | Stock status |
| quantity | Quantity per unit |

---

## 🧹 Data Cleaning

- Removed products with `MRP = 0`  
- Converted prices from paise to rupees  
- Checked NULL values  
- Identified duplicate products  

---

## 🔍 Data Exploration

- Total number of products  
- Unique categories  
- Stock availability (in-stock vs out-of-stock)  
- Duplicate product analysis  

---

## 📊 Key Business Insights

### 1. Top Discounted Products
Identified products with highest discount percentages.

### 2. High-Value Out-of-Stock Products
Products with:
- MRP > ₹300  
- Currently out of stock  

### 3. Category-wise Revenue
Estimated total revenue using:

`SUM(discountedSellingPrice * availableQuantity)`

---

### 4. Premium Low-Discount Products
Filtered products where:
- MRP > ₹500  
- Discount < 10%  

---

### 5. Best Discount Categories
Identified top 5 categories offering the highest average discount.

---

### 6. Price Efficiency
Calculated **price per gram** to determine best-value products.

---

### 7. Product Segmentation
Products categorized based on weight:

- Low weight (< 1kg)  
- Medium weight (1kg–5kg)  
- Bulk (> 5kg)  

---

### 8. Inventory Weight Analysis
Calculated total inventory weight for each category.

---

## 🧠 Key Learnings

- Writing advanced SQL queries:
  - GROUP BY  
  - HAVING  
  - CASE WHEN  
- Performing real-world data cleaning  
- Extracting business insights from raw data  
- Understanding e-commerce analytics  

---

## 🛠️ Tech Stack

- SQL (MySQL / PostgreSQL)  
- MySQL Workbench / pgAdmin  

---

## 🚀 How to Run

1. Create a database  
2. Import the SQL file  
3. Run queries  

Example:
`SOURCE zepto_project.sql;`

---

## 📈 Future Improvements

- Build Power BI / Tableau dashboard  
- Add Python (Pandas) analysis  
- Perform time-series analysis  
- Apply machine learning models  

---

## 👨‍💻 About the Author
Hey, I’m Nitish Gope — a Data Analyst. I break down complex data topics into simple, practical content that actually helps you land a job.

---

## 🤝 Connect With Me

- LinkedIn: [Nitish Gope](https://www.linkedin.com/in/nitish-gope-58370a236/)
---

## ⭐ Support

If you found this useful, consider giving it a ⭐ on GitHub!

