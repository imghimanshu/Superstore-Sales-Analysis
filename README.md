# 🛒 Superstore Sales Analysis

Exploratory Data Analysis (EDA) of the Superstore sales dataset, uncovering sales, profit, and product trends using Python, pandas, and data visualization.

---

## 📌 Overview

This project analyzes retail sales data from a fictional "Superstore" to understand what drives revenue and profit across categories, regions, and products. Using **pandas** for data wrangling and **matplotlib/seaborn** for visualization, the notebook walks through cleaning, aggregating, and charting the dataset to surface actionable business insights — the kind of analysis a retail analytics or BI team would use to guide inventory, pricing, and regional strategy decisions.

---

## 📊 Dataset

- **Source**: Superstore Sales dataset (originally from Kaggle)
- **Records**: 9,994 orders
- **Columns**: 22 fields including Order Date, Ship Date, Ship Mode, Customer, Segment, Region, Category, Sub-Category, Product Name, Sales, Quantity, Discount, and Profit
- **Files**:
  - `data/raw/superstore_clean.csv` — original dataset as downloaded
  - `data/cleaned/Himanshu_clean.csv` — cleaned dataset used in the analysis (parsed dates, consistent formatting)

---

## 🔑 Key Insights

- **Technology** is the top-selling category ($836K), narrowly ahead of **Furniture** ($742K) and **Office Supplies** ($719K) — but sales volume alone doesn't tell the profit story.
- The **West** region is the most profitable ($108K profit), followed by **East** ($92K), while **South** ($47K) and **Central** ($40K) lag well behind — a >2.5x gap between the best and worst-performing regions.
- Monthly sales show a clear **seasonal pattern**, with recurring peaks toward the end of the calendar year, suggesting strong Q4 demand (holiday season effect).
- A handful of products — like the **HP Designjet T520 printer** and **Canon imageCLASS copier** — drive a disproportionate share of total profit, highlighting the value of hero-product focus.
- The Category × Sub-Category heatmap reveals that profit and sales performance is uneven *within* categories — some sub-categories carry a category's whole performance while others barely contribute.

---

## 🔍 Key Analysis & Findings

1. **Total Sales by Category** — Bar chart comparing summed sales across Technology, Furniture, and Office Supplies.
   ![Sales by Category](outputs/sales_by_category.png)

2. **Monthly Sales Trend** — Line chart tracking sales over time, revealing seasonality and growth patterns.
   ![Monthly Sales Trend](outputs/monthly_trend.png)

3. **Total Profit by Region** — Bar chart showing which regions generate the most (and least) profit.
   ![Profit by Region](outputs/profit_by_region.png)

4. **Sales Heatmap (Category vs Sub-Category)** — Cross-tabulation showing exactly where revenue concentrates at the sub-category level.
   ![Sales Heatmap](outputs/heatmap.png)

5. **Top 10 Products by Profit** — Horizontal bar chart ranking the most profitable individual products.
   ![Top 10 Products by Profit](outputs/top10_products.png)

---

## 🛠️ Technologies Used

- **Python 3** — core programming language
- **pandas** — data loading, cleaning, grouping, and aggregation
- **matplotlib** — bar charts, line charts, and horizontal bar charts
- **seaborn** — heatmap visualization
- **Jupyter Notebook** — interactive analysis environment
- **NumPy** *(pandas dependency)* — numerical operations

---

## 💡 Why This Project Matters

Retail and e-commerce businesses generate huge volumes of transactional data, but raw numbers alone don't drive decisions — clear, well-visualized insights do. This project demonstrates a complete, real-world EDA workflow: taking messy raw sales data, cleaning it, and turning it into charts that answer concrete business questions like *"Which region should we invest in?"* and *"Which products should we double down on?"*

It reflects core data analyst skills that transfer directly to any business setting — data cleaning, aggregation, visualization, and translating numbers into a narrative decision-makers can act on.

---

## ⚙️ Setup

```bash
pip install -r requirements.txt
jupyter notebook superstore_analysis.ipynb
```

## 📁 Project Structure

```
superstore-sales-analysis/
├── README.md
├── requirements.txt
├── superstore_analysis.ipynb
├── data/
│   ├── raw/superstore_clean.csv
│   └── cleaned/Himanshu_clean.csv
└── outputs/
    ├── sales_by_category.png
    ├── monthly_trend.png
    ├── profit_by_region.png
    ├── heatmap.png
    └── top10_products.png
```
