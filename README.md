# 🧾 SuperStore Sales Analysis

This repository contains the **complete SuperStore Sales & Retail Orders analysis project**, originally created by **Hemanshu** and organized into a reproducible Python–Power BI workflow by **Siddhesh Ashok Gaikwad**.

It includes **raw data**, **cleaned datasets**, **Power BI dashboard reference**, and **Python scripts** used to clean and analyze the data with Pandas.

---

## 📂 Repository Structure

SuperStore_Sales_Analysis/
│
├── data/
│ ├── raw/
│ │ ├── SuperStoreOrders.csv
│ │ ├── Retail_orders.csv
│ │ └── Sales_Data_Dashboard.PBI-1.pdf
│ │
│ └── cleaned/
│ ├── cleaned_SuperStoreOrders.csv
│ ├── cleaned_Retail_orders.csv
│ └── combined_cleaned_orders.csv
│
├── src/
│ └── cleaning.py
│
├── notebooks/
│ └── 01-data-cleaning.md
│
├── powerbi/
│ └── Sales_Data_Dashboard.PBI-1.pdf
│
├── reports/
│ └── metrics.md
│
├── requirements.txt
├── LICENSE
└── README.md

---

## 🧠 Project Overview

This project demonstrates **end-to-end sales analysis** from raw CSV data to a **Power BI dashboard**.

- Cleaned and combined **SuperStore Orders** and **Retail Orders** datasets  
- Used **Python (Pandas)** for cleaning, validation, and feature engineering  
- Created **Power BI dashboard** for visual insights on sales, profit, and performance  
- Integrated cleaned data for **interactive analytics and business insights**

---

## 🧹 Data Cleaning Process

The data cleaning and transformation were done entirely in **Python using Pandas**.

**Steps performed:**
1. Standardized column names (lowercase, underscores, no special chars)  
2. Parsed all date columns automatically (`order_date`, `ship_date`)  
3. Converted numeric-like columns (sales, profit, quantity, etc.) to proper numeric types  
4. Removed duplicate rows  
5. Added new calculated columns:
   - `order_year`, `order_month`, `order_day`  
   - `profit_margin = profit / sales`
6. Exported cleaned datasets to `data/cleaned/`

---

## 🧾 Datasets

| File Name | Rows | Columns | Description |
|------------|------|----------|-------------|
| **SuperStoreOrders.csv** | 51,290 | 25 | Original SuperStore data |
| **Retail_orders.csv** | 51,290 | 28 | Retail data version |
| **combined_cleaned_orders.csv** | 102,580 | 28 | Merged dataset for unified analysis |

---

## 📊 Power BI Dashboard

The **Power BI dashboard** (created by Hemanshu) is available as a PDF for reference:

📁 `powerbi/Sales_Data_Dashboard.PBI-1.pdf`

It visualizes:
- Total Sales & Profit  
- Region-wise performance  
- Segment & Category analysis  
- Yearly and Monthly trends  
- Profit Margin comparison  

---

## 🧮 Key Metrics (in Python & DAX)

**Python (Pandas)**
```python
total_sales = df['sales'].sum()
total_profit = df['profit'].sum()
qty_sold = df['quantity'].sum()
df['profit_margin'] = df['profit'] / df['sales']

## 👨‍💻 Authors

| Name | Role | Description |
|------|------|--------------|
| 🧠 **Himanshu**( https://github.com/Himanshu76-DA ) |  Data cleaning, Python integration, Power BI Developer | Created the full Power BI Dashboard |
| 👨‍💻 **Siddhesh Ashok Gaikwad**( https://github.com/siddheshDA ) | Data Analyst & Developer | and repository setup |

---

## ⚙️ Tools Used

| Tool | Purpose |
|------|----------|
| 🐍 **Python (Pandas, NumPy)** | Data cleaning and transformation |
| 📊 **Power BI** | Dashboard creation and visualization |
| 📓 **Jupyter / Markdown** | Data exploration and documentation |
| 💾 **GitHub** | Repository hosting and version control |
