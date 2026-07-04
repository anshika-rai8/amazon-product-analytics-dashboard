# Amazon Product Analytics Dashboard

## 📌 Project Overview

The goal of this project is to clean, transform, analyze, and visualize Amazon product data to uncover insights about:

- 📦 Product Categories
- ⭐ Customer Ratings
- 💰 Product Pricing
- 🏷️ Discounts

The project demonstrates the complete data analytics workflow—from raw data to an interactive dashboard.

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
Power BI Dashboard
      │
      ▼
Business Insights
```

## 📊 Dashboard Preview

![Dashboard](dashboard.png)

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

## 📈 Key Insights

- Electronics contains the highest number of products.
- Home Improvement has the highest average discount.
- Office Products has the highest average rating.

## 📁 Project Structure

```text
Amazon-Product-Analytics/
│
├── Amazon_Product_Analysis.ipynb
├── amazon_cleaned.csv
├── Amazon_Dashboard.pbix
├── dashboard.png
├── README.md
├── requirements.txt
```

## 🚀 Skills Demonstrated

- Data Cleaning
- Data Transformation
- Exploratory Data Analysis
- Data Visualization
- Dashboard Design
- Business Insight Generation
- Power BI Reporting

## 📁 Project Files

- [📓 Jupyter Notebook](amazon_product_analytics.ipynb)
- [📊 Cleaned Dataset](amazon_cleaned.csv)
- [📈 Power BI Dashboard](amazon_dashboard.pbix)
- [🖼️ Dashboard Screenshot](Dashboard.png)
