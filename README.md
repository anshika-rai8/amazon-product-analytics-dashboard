# Amazon Product Analytics Dashboard

## 📌 Project Overview

The goal of this project is to clean, transform, analyze, and visualize Amazon product data to uncover insights about:

- 📦 Product Categories
- ⭐ Customer Ratings
- 💰 Product Pricing
- 🏷️ Discounts

The project demonstrates the complete data analytics workflow — from raw data to an interactive dashboard, including a statistical check on sample size before drawing conclusions.

## 🛠️ Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Power BI

## 📂 Project Workflow

```text
Raw Dataset
      │
      ▼
Data Cleaning (Python)
      │
      ▼
Exploratory Data Analysis (EDA)
      │
      ▼
Sample-Size Validation
      │
      ▼
Power BI Dashboard
      │
      ▼
Business Insights
```

## 📊 Dashboard Preview

### Page 1 — Overview
![Dashboard Overview](Amazon_dashboard_pg1.png)

### Page 2 — Discount vs. Rating Analysis
![Discount vs Rating Analysis](Amazon_dashboard_pg2.png)

## 🔍 Data Cleaning

The dataset was cleaned by:

- Removing missing values
- Checking duplicate rows
- Cleaning price columns (₹ symbol and commas)
- Converting data types
- Cleaning percentage values
- Handling invalid rating values
- Creating a new `main_category` column

## 📈 Exploratory Data Analysis

The analysis focused on:

- Products by Category
- Average Rating by Category
- Average Discount by Category
- Price Analysis
- Correlation between Rating and Discount

## ⚠️ Sample-Size Validation

- The raw dataset contains 9 categories, but 5 of them (MusicalInstruments, HomeImprovement, Car&Motorbike, Health&PersonalCare, Toys&Games) had 2 or fewer products each — in three cases, just a single listing. Category-level averages from such small samples aren't statistically meaningful and can be misleading if compared alongside categories with hundreds of products.

- To keep the analysis honest, all category-level comparisons (rating, discount, product count) were filtered to categories with 30+ products, leaving four categories with real statistical weight: Electronics, Computers&Accessories, Home&Kitchen, and OfficeProducts — together representing over 97% of the dataset.

## 📈 Key Insights
(based on categories with 30+ products; n = sample size)

- Electronics has the highest product volume (n = 526), followed closely by Computers&Accessories (n = 451) and Home&Kitchen (n = 447).
- Computers&Accessories offers the deepest average discount (53.9%) among high-volume categories, while also holding the second-highest average rating (4.16) — the strongest combination of scale, savings, and satisfaction in the dataset.
- OfficeProducts (n = 31) has the highest average rating (4.31) despite the lowest average discount (12.4%) — suggesting customer satisfaction here isn't being bought with markdowns.
- Across the full dataset, the correlation between discount percentage and rating is weak (r ≈ -0.16) — deeper discounts do not meaningfully predict higher or lower customer ratings.
- Categories with very few listings (MusicalInstruments, HomeImprovement, Car&Motorbike, Health&PersonalCare, Toys&Games) were excluded from category-level comparisons due to insufficient sample size, though they remain in the raw dataset and filterable in the dashboard.

## 📁 Project Structure

```text
Amazon-Product-Analytics/
│
├── Amazon_Product_Analysis.ipynb
├── amazon_cleaned.csv
├── Amazon_Dashboard.pbix
├── Amazon dashboard pg1.png
├── Amazon dashboard pg2.png
├── README.md
├── requirements.txt
```

## 🚀 Skills Demonstrated

- Data Cleaning
- Data Transformation
- Exploratory Data Analysis
- Statistical Reasoning (sample-size validation, correlation analysis)
- Data Visualization
- Dashboard Design
- Business Insight Generation
- Power BI Reporting

## 📁 Project Files

- [📓 Jupyter Notebook](amazon_product_analytics.ipynb)
- [📊 Cleaned Dataset](amazon_cleaned.csv)
- [📈 Power BI Dashboard](amazon_dashboard.pbix)
- [🖼️ Dashboard Screenshot page 1](Amazon_dashboard_pg1.png)
- [🖼️ Dashboard Screenshot page 2](Amazon_dashboard_pg2.png)
