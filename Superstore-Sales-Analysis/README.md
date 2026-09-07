# 📊 Superstore Sales & Profitability Analysis

An end-to-end exploratory data analysis project on retail sales data — cleaning, feature engineering, statistical analysis, visualization, and automated business reporting, built entirely with **Pandas, NumPy, Matplotlib, and Seaborn**.

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

## 🧭 Overview

A retail company (Superstore) wants to understand its sales performance, profitability, customer behavior, and shipping efficiency across categories, regions, and segments — and to automate this reporting instead of doing it manually every time.

This project builds a complete, reusable analysis workflow that:
- Cleans and validates ~10,000 order records
- Engineers new business metrics (profit margin, shipping duration, sales tier)
- Explores the data through 12 visualizations
- Runs correlation and distribution analysis
- Automatically generates a KPI summary and a written business report

## 📁 Dataset

**Source:** Sample - Superstore 2019 (`Orders` sheet)
**Size:** 9,994 rows × 21 columns
**Fields:** Order/Ship dates, Customer, Segment, Region, Product Category, Sales, Quantity, Discount, Profit, and more.

## 🔑 Key Business Insights

| Metric | Value |
|---|---|
| Total Sales | **$2,297,200.86** |
| Total Profit | **$286,397.02** |
| Overall Profit Margin | **12.47%** |
| Total Orders | 5,009 |
| Total Customers | 793 |
| Average Shipping Duration | 3.96 days |
| Top Category (Sales & Profit) | **Technology** |
| Top Region (Sales) | **West** |

- **Technology** is both the best-selling and most profitable category — a strong core of the business.
- There is a **negative correlation between Discount and Profit**: higher discounts tend to come with lower profit.
- A small set of products account for repeated **negative profit**, flagging a pricing/discount issue worth investigating.
- A handful of top customers drive a disproportionate share of revenue — good loyalty-program candidates.

## 📈 Sample Visualizations

| | |
|---|---|
| ![Sales by Category](visualizations/03_sales_by_category.png) | ![Correlation Heatmap](visualizations/10_correlation_heatmap.png) |
| ![Monthly Sales Trend](visualizations/06_monthly_sales_trend.png) | ![Discount vs Profit](visualizations/09_discount_vs_profit.png) |

*(All 12 charts are available in the [`visualizations/`](visualizations) folder.)*

## 🛠️ Methodology

1. **Data Cleaning** — missing values, duplicates, data types, text formatting, IQR-based outlier detection (kept, not removed, to preserve real large orders)
2. **Reusable Preprocessing Functions** — modular functions for cleaning steps that can run on any similar dataset
3. **Feature Engineering** — `Profit Margin`, `Shipping Duration`, `Sales Performance Category`
4. **Object-Oriented Design** — a `SuperstoreAnalyzer` class for core KPI/grouping logic
5. **Exploratory Data Analysis** — sales, profit, customer, product, and shipping breakdowns
6. **Statistical Analysis** — correlation matrix, distribution shape, monthly trend analysis
7. **Visualization** — 12 labeled charts (histograms, bar charts, line trends, scatter plots, heatmap)
8. **Automated Reporting** — KPI table + text report generated directly from the data
9. **Memory Optimization** — `category` dtype conversion to reduce memory footprint
10. **Export Pipeline** — cleaned dataset, KPI summary, and report auto-saved to disk

## 🧰 Tech Stack

- Python 3
- Pandas & NumPy — data manipulation
- Matplotlib & Seaborn — visualization
- Jupyter Notebook — analysis environment

## 📂 Repository Structure

```
Superstore-Sales-Analysis/
│
├── notebook/
│   └── Superstore_Mini_Project_1.ipynb   # Full analysis, step by step
│
├── data/
│   └── Sample_-_Superstore_2019.xls      # Raw dataset
│
├── outputs/
│   ├── cleaned_superstore.csv            # Cleaned & feature-engineered data
│   ├── kpi_summary.csv                   # Automated KPI table
│   └── analytical_report.txt             # Automated business report
│
├── visualizations/                       # All 12 exported charts (PNG)
│
├── requirements.txt
└── README.md
```

## ▶️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/Superstore-Sales-Analysis.git
cd Superstore-Sales-Analysis

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch the notebook
jupyter notebook notebook/Superstore_Mini_Project_1.ipynb
```

## 💡 Skills Demonstrated

`Data Cleaning` `Feature Engineering` `Object-Oriented Programming` `Exception Handling` `Exploratory Data Analysis` `Statistical Analysis (Correlation)` `Data Visualization` `Automated Reporting` `Memory Optimization`

---

**Author:** [Your Name] — feel free to connect on [LinkedIn](#) or check out my other projects.
