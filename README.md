# 🛒 Zepto SQL Data Analysis Project

## 🔗 Data Source & Context

This project is inspired by real-world quick-commerce operations like **Zepto**, focusing on product pricing, discounts, inventory, and revenue analytics.

- 🛒 Zepto Platform: https://www.zeptonow.com/
- 📊 Dataset Source (Kaggle): https://www.kaggle.com/your-dataset-link  

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
| sku_id | Unique product ID |
| category | Product category |
| name | Product name |
| mrp | Maximum Retail Price (₹) |
| discountPercent | Discount % |
| availableQuantity | Available stock |
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
Estimated using:
```sql
SUM(discountedSellingPrice * availableQuantity)
