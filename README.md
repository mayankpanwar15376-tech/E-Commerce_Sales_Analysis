# 🛒 E-Commerce Sales & Profit Analysis

An exploratory data analysis of a 3-year retail transaction dataset, uncovering sales trends, profit drivers, and underperforming product lines to support data-driven business decisions.

**Dataset: 9,994 orders | $2.30M total sales | $286K total profit | 2014–2017**

---

## 📌 Overview

This project analyzes a retail superstore's order-level transaction data to answer key business questions:
- Which months drive the most sales and profit?
- Which product categories and sub-categories are the strongest — and weakest — performers?
- How do different customer segments compare in sales and profitability?

The analysis moves from raw transactional data to time-based feature engineering, category-level aggregation, and segment profitability comparisons.

---

## 📊 Dataset

- **Source:** Sample Superstore dataset — 9,994 order line items across 21 columns
- **Time range:** January 2014 – December 2017
- **Key fields:** Order Date, Ship Date, Segment, Category, Sub-Category, Region, Sales, Profit, Discount, Quantity

---

## ⚙️ Feature Engineering

Date fields were parsed and decomposed to enable time-based analysis:
- `Order Month`, `Order Year` — extracted from `Order Date`
- `Order Day of Week` — extracted for weekday pattern analysis

---

## 📈 Sales Analysis

**Monthly sales show a clear seasonal ramp-up toward year-end**, with November and December consistently the strongest months — a classic holiday-shopping pattern.

![Monthly Sales Analysis](images/monthly_sales.png)

**Category breakdown** shows Technology and Office Supplies leading sales share:

![Sales by Category](images/sales_by_category.png)

**Phones and Chairs are the top-selling sub-categories**, while several sub-categories lag well behind:

![Sales by Sub-Category](images/sales_by_subcategory.png)

---

## 💰 Profit Analysis

Profit doesn't always track sales — some high-selling sub-categories are actually **losing money**:

![Monthly Profit Analysis](images/monthly_profit.png)

**Tables is the single most unprofitable sub-category** in the entire dataset (–$17,725 total loss), despite reasonable sales volume — a strong signal for pricing or discount-strategy review.

![Profit by Sub-Category](images/profit_by_subcategory.png)

---

## 👥 Customer Segment Analysis

| Segment | Total Sales | Total Profit | Sales-to-Profit Ratio |
|---|---|---|---|
| Consumer | $1,161,401 | $134,119 | 8.66 |
| Corporate | $706,146 | $91,979 | 7.68 |
| Home Office | $429,653 | $60,299 | 7.13 |

**Home Office has the most efficient sales-to-profit ratio**, converting revenue into profit more effectively than the larger Consumer segment — despite having the smallest sales volume overall.

![Sales and Profit by Segment](images/sales_profit_by_segment.png)

---

## 🔑 Key Takeaways

- **Seasonality is strong** — sales and marketing efforts are best concentrated in Q4.
- **The Tables sub-category is actively losing money** and warrants a pricing, sourcing, or discount policy review.
- **Consumer segment drives the most revenue**, but **Home Office is the most profit-efficient** — worth investing more in relative to its current sales share.

---

## 🛠️ Tech Stack

- **Language:** Python
- **Data handling:** Pandas
- **Visualization:** Plotly Express, Plotly Graph Objects (interactive charts in the notebook)

---

## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/mayankpanwar15376-tech/E-commerce-Sales-Analysis.git
cd E-commerce-Sales-Analysis

# Install dependencies
pip install pandas plotly

# Launch the notebook
jupyter notebook E-commerce_project.ipynb
```

---

## 📁 Repository Structure

```
├── E-commerce_project.ipynb   # Full analysis notebook
├── Sample_-_Superstore.csv    # Dataset
├── images/                    # Chart exports used in this README
└── README.md
```

---

## 📈 Possible Next Steps

- Build a discount-vs-profit analysis to quantify how discounting erodes margin by sub-category
- Add regional analysis (Sales/Profit by Region and State) to identify geographic opportunities
- Turn this into an interactive Power BI / Tableau dashboard for stakeholder use

---

## 👤 Author

**Mayank Panwar**
[GitHub](https://github.com/mayankpanwar15376-tech) · [LinkedIn](https://www.linkedin.com/in/mayank-panwar-9a988725a)
