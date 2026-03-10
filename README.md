# 🛍️ Customer Shopping Behavior Analysis

A data analysis project that explores transactional shopping data to uncover insights into customer spending patterns, product preferences, and subscription behavior — using **Python**, **PostgreSQL**, and **Power BI**.

---

## 📌 Project Overview

This project analyzes **3,900 purchase transactions** across multiple product categories. The goal is to support strategic business decisions by identifying customer segments, revenue drivers, and discount dependencies.

---

## 📁 Dataset Summary

| Property | Details |
|---|---|
| Rows | 3,900 |
| Columns | 18 |
| Missing Data | 37 values in `review_rating` column |

**Key Features:**
- **Customer Demographics:** Age, Gender, Location, Subscription Status
- **Purchase Details:** Item Purchased, Category, Purchase Amount, Season, Size, Color
- **Shopping Behavior:** Discount Applied, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python (pandas) | Data cleaning & feature engineering |
| PostgreSQL | SQL-based business analysis |
| Power BI | Interactive dashboard & visualization |

---

## 🔍 Exploratory Data Analysis (Python)

Data preparation steps performed in Python:

- **Data Loading** – Imported dataset using `pandas`
- **Initial Exploration** – Used `df.info()` and `.describe()` for structure and summary statistics
- **Missing Data Handling** – Imputed missing `review_rating` values using the median rating per product category
- **Column Standardization** – Renamed all columns to `snake_case`
- **Feature Engineering:**
  - Created `age_group` column by binning customer ages
  - Created `purchase_frequency_days` column from purchase data
- **Data Consistency Check** – Verified redundancy between `discount_applied` and `promo_code_used`; dropped `promo_code_used`
- **Database Integration** – Loaded cleaned DataFrame into PostgreSQL for SQL analysis

---

## 📊 SQL Business Analysis (PostgreSQL)

Ten business questions were answered using structured SQL queries:

| # | Analysis | Key Finding |
|---|---|---|
| 1 | Revenue by Gender | Male: $157,890 · Female: $75,191 |
| 2 | High-Spending Discount Users | 839 customers spent above average despite using discounts |
| 3 | Top 5 Products by Rating | Gloves (3.86), Sandals (3.84), Boots (3.82), Hat (3.80), Skirt (3.78) |
| 4 | Shipping Type Comparison | Express avg: $60.48 · Standard avg: $58.46 |
| 5 | Subscribers vs. Non-Subscribers | Similar avg spend (~$59.50 vs ~$59.87) |
| 6 | Discount-Dependent Products | Hat (50%), Sneakers (49.66%), Coat (49.07%) |
| 7 | Customer Segmentation | Loyal: 3,116 · Returning: 701 · New: 83 |
| 8 | Top 3 Products per Category | Jewelry, Blouse, Sandals, Jacket lead their categories |
| 9 | Repeat Buyers & Subscriptions | 2,518 non-subscribers vs 958 subscribers among repeat buyers |
| 10 | Revenue by Age Group | Young Adult: $62,143 · Middle-aged: $59,197 |

---

## 📈 Power BI Dashboard

An interactive dashboard was built to visualize key metrics:

- KPI cards: Total Customers, Avg Purchase Amount, Avg Review Rating
- % of Customers by Subscription Status (donut chart)
- Sales & Revenue by Category and Age Group (bar charts)
- Slicers for Gender, Category, Subscription Status, and Shipping Type

---

## 💡 Business Recommendations

1. **Boost Subscriptions** – Promote exclusive member benefits to convert the 73% non-subscriber base
2. **Customer Loyalty Programs** – Reward repeat buyers to accelerate movement into the "Loyal" segment
3. **Review Discount Policy** – Balance sales volume gains with margin impact, especially for Hat and Sneakers
4. **Product Positioning** – Feature top-rated products (Gloves, Sandals) prominently in marketing campaigns
5. **Targeted Marketing** – Focus on Young Adult and Middle-aged age groups, the highest revenue contributors



