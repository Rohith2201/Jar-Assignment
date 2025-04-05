# 📊 Jar DSA Assignment

## Overview

This project focuses on **Sales and Profitability Analysis**, **Target Achievement Analysis**, and **Regional Performance Insights** using three datasets provided:

- `Order_Details_19795F61CF.csv`
- `Sales_target_DD2E9B96A0.csv`
- `List_of_Orders_55FFC79CF8.csv`

The goal is to derive meaningful business insights through data analysis and visualization using Python, Pandas, and Seaborn.

---

## 🔧 Technologies Used

- **Python**
- **Pandas** — data manipulation and analysis
- **Seaborn & Matplotlib** — data visualization
- **Jupyter Notebook / IPython**

---

## 📂 Dataset Details

- **Order Details**: Includes product-wise sales and profit information.
- **Sales Target**: Monthly target sales for each category.
- **List of Orders**: Contains order-level and regional information.

---

## ✅ Part 1: Sales and Profitability Analysis

### Tasks Performed:

- Merged Order Details and List of Orders on `Order ID`.
- Calculated **total sales per category**.
- Computed:
  - **Average profit per order** for each category.
  - **Profit margin** = Profit ÷ Amount × 100.

### Key Insights:

| Category     | Total Sales | Avg Profit/Order | Profit Margin (%) |
|--------------|-------------|------------------|--------------------|
| Clothing     | 139,054     | 11.76            | 8.03               |
| Electronics  | 165,267     | 34.07            | 6.35               |
| Furniture    | 127,181     | 9.45             | 1.81               |

- 📈 **Top-performing category**: **Clothing**
- ⚠️ **Underperforming category**: **Furniture**

#### Possible Reasons:
- Higher demand and margins in fashion segment.
- Furniture may have high logistics/handling costs reducing margins.

---

## 📈 Part 2: Target Achievement Analysis

### Objective:

- Analyzed **month-over-month percentage change** in sales target for **Furniture** category.

### Highlights:

- Monthly changes hovered around 0.87%–1.88%.
- ✅ **No significant fluctuations (>20%)** were observed, indicating steady sales targets.

### Visualization:

- 📊 Line plot of percentage change in targets over time.

---

## 🌍 Part 3: Regional Performance Insights

### Top 5 States (by Order Count):

- Madhya Pradesh
- Maharashtra
- Rajasthan
- Gujarat
- Punjab

### Metrics Calculated:

| State            | Total Sales | Avg Profit |
|------------------|-------------|------------|
| Madhya Pradesh   | 105,140     | 16.33      |
| Maharashtra      | 95,348      | 21.30      |
| Rajasthan        | 21,149      | 16.99      |
| Gujarat          | 21,058      | 5.34       |
| Punjab           | 16,786      | -10.15     |

### Underperforming Regions:
- **Punjab**: Negative average profit (likely due to high discounts or returns).
- **Gujarat**: Lowest profit margin among profitable regions.

---

## ⚠️ Notes

- **Warnings from Seaborn**: Future deprecation notices for `palette` usage without `hue`. To resolve, add `hue=x` and `legend=False` or upgrade to newer Seaborn practices.
- **Pandas Warning**: Avoid chained assignments when using `.fillna(inplace=True)`.

---

## 📌 Conclusion

This analysis provides crucial business intelligence into product category performance, target trends, and regional disparities. Such insights can guide marketing strategies, inventory planning, and resource allocation for improved profitability.

---

Let me know if you want this exported as a PDF or added to a Jupyter Notebook!
