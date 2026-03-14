# Amazon Sales — Python Exploratory Data Analysis (EDA)



## Project Overview

This project performs an in-depth **Exploratory Data Analysis (EDA)** on Amazon sales data using Python. It covers 8 structured business questions, progressing from high-level sales performance down to customer behaviour and correlation analysis — producing publication-ready visualisations at every stage.

---


##  Dataset Overview

| Column | Description |
|---|---|
| `order_id` | Unique order identifier |
| `order_date` | Date the order was placed |
| `product_category` | Top-level product category |
| `price` | Original product price ($) |
| `discount_percent` | Discount applied (%) |
| `discounted_price` | Final price after discount ($) |
| `quantity_sold` | Number of units sold per order |
| `total_revenue` | Actual revenue generated ($) |
| `customer_region` | Geographic region of the customer |
| `rating` | Customer product rating |
| `review_count` | Number of reviews for the product |

---

##  EDA Questions Covered

| # | Question | Focus Area |
|---|---|---|
| Q1 | Overall Sales Performance | Total revenue, orders, avg order value, discount rate |
| Q2 | Sales Trend Over Time | Monthly revenue trend with peak annotation |
| Q3 | Category Performance | Revenue vs discount cost by product category |
| Q4 | Top Category Analysis | Top 5 categories by revenue and by discount given |
| Q5 | Regional Performance | Revenue, orders, avg order value, and rating by region |
| Q6 | Profitability & Discount Analysis | Revenue and avg order value by category |
| Q7 | Customer Purchasing Behaviour | Order quantity distribution and patterns |
| Q8 | Relationship Analysis | Correlation matrix across all key numeric variables |

---

##  Visualisations Produced

-  Area + Line chart — Monthly Revenue Trend (with peak annotation)
-  Horizontal stacked bar — Revenue vs Discount Cost by Category
-  Side-by-side bar charts — Top 5 Categories by Revenue & Discount
-  Correlation Heatmap — All key numeric variables (Blues palette)

---

##  Key Highlights

- Revenue, quantity, pricing, and discount data cleaned and analysed across all product categories
- Time features engineered from `order_date`: `year`, `month`, `month_name`, `month_year`
- Discount impact assessed at both category and regional levels
- Correlation analysis reveals relationships between price, discount, quantity, revenue, rating, and review count
- All charts exported as high-resolution `.png` files (150 DPI)

---

##  Libraries Used

| Library | Purpose |
|---|---|
| `pandas` | Data loading, cleaning, and aggregation |
| `numpy` | Numerical operations and correlation matrix masking |
| `matplotlib` | Core charting and custom formatting |
| `seaborn` | Correlation heatmap visualisation |
| `warnings` | Suppressing non-critical runtime warnings |

---

##  How to Run

1. Clone this repository
2. Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn
```
3. Place `amazon_sales_dataset.csv` in your working directory
4. Open and run `Amazon_Sales_EDA.ipynb` cell by cell in Jupyter Notebook or VS Code

```python
# Quick start — load and preview the dataset
import pandas as pd
df = pd.read_csv('amazon_sales_dataset.csv')
df.head()
```

---

##  Colour Palette Used

| Variable | Hex | Usage |
|---|---|---|
| Navy | `#1B3A6B` | Primary bars and lines |
| Teal | `#0D7377` | Supporting visual elements |
| Gold | `#F4A300` | Discount highlights and accents |

---

