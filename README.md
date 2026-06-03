# Restaurant Sales Analysis with Python

## Project Overview

This project analyzes restaurant sales data using Python, Pandas, NumPy, and Matplotlib. The objective is to clean the dataset, perform exploratory data analysis (EDA), and identify key business insights related to sales performance, customer payment preferences, products, managers, and cities.

---

## Business Questions

The analysis aims to answer the following questions:

1. What is the most preferred payment method?
2. Which product sells the most by quantity?
3. Which product generates the highest revenue?
4. Which city generates the highest revenue?
5. Which manager generates the highest revenue?
6. How does revenue change over time?
7. What is the average revenue per transaction?
8. How does average revenue compare between November and December?

---

## Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Jupyter Notebook

---

## Data Cleaning Process

The raw dataset contained several data quality issues:

### 1. Removed Unnecessary Columns

* Dropped the empty column `Unnamed: 0`.

### 2. Fixed Column Headers

* Promoted the first row to become the dataset header.

### 3. Standardized Manager Names

* Removed leading/trailing spaces.
* Replaced multiple spaces with a single space.

Example:

* `Tom      Jackson` → `Tom Jackson`
* `Joao    Silva` → `Joao Silva`

### 4. Removed Duplicate Records

* Identified and removed duplicate rows.

### 5. Corrected Product Prices

Incorrect prices were detected and replaced:

| Incorrect Price | Correct Price |
| --------------- | ------------- |
| 25.50           | 3.49          |
| 29.05           | 9.95          |

### 6. Converted Data Types

| Column   | Data Type |
| -------- | --------- |
| Order ID | Integer   |
| Date     | Datetime  |
| Price    | Float     |
| Quantity | Integer   |

### 7. Created Revenue Column

Revenue was calculated using:

Revenue = Price × Quantity

---

## Key Findings

### 1. Most Preferred Payment Method

| Payment Method | Transactions |
| -------------- | ------------ |
| Credit Card    | 120          |
| Cash           | 76           |
| Gift Card      | 58           |

**Insight:** Credit Card is the most preferred payment method, accounting for approximately 47.24% of all transactions.

---

### 2. Top Selling Products by Quantity

| Product            | Quantity Sold |
| ------------------ | ------------: |
| Beverages          |        34,938 |
| Fries              |        32,016 |
| Burgers            |        28,996 |
| Chicken Sandwiches |        11,132 |
| Sides & Other      |         9,800 |

**Insight:** Beverages are the highest-selling product by quantity.

---

### 3. Top Revenue-Generating Products

| Product            |     Revenue |
| ------------------ | ----------: |
| Burgers            | $376,658.04 |
| Fries              | $111,735.84 |
| Chicken Sandwiches | $110,763.40 |
| Beverages          | $103,067.10 |
| Sides & Other      |  $48,902.00 |

**Insight:** Burgers generate the highest revenue despite not having the highest sales volume.

---

### 4. Revenue by City

| City   |     Revenue |
| ------ | ----------: |
| Lisbon | $223,803.98 |
| London | $211,001.83 |
| Madrid | $136,098.22 |
| Berlin | $100,492.73 |
| Paris  |  $79,729.62 |

**Insight:** Lisbon contributes the highest total revenue.

---

### 5. Revenue by Manager

| Manager       |     Revenue |
| ------------- | ----------: |
| Joao Silva    | $223,803.98 |
| Tom Jackson   | $211,001.83 |
| Pablo Perez   | $136,098.22 |
| Walter Muller | $100,492.73 |
| Remy Monet    |  $79,729.62 |

**Insight:** Joao Silva is the top-performing manager in terms of revenue generation.

---

### 6. Revenue Trend Analysis

Revenue was aggregated by date and visualized using a line chart.

**Insight:** Daily revenue fluctuates significantly throughout the analysis period, indicating variations in customer demand.

---

### 7. Average Revenue per Transaction

Average Revenue:

$2,957.19

---

### 8. Average Revenue by Month

| Month    | Average Revenue |
| -------- | --------------: |
| November |       $2,779.97 |
| December |       $3,099.22 |

**Insight:** December achieved a higher average revenue than November, suggesting stronger sales performance during the holiday season.

---

## Project Structure

```text
Restaurant-Sales-Analysis-Python
│
├── Restaurant_Sales_Analysis.ipynb
├── Sales-Data-Analysis.xlsx
├── README.md
│
├── images
│   ├── payment_method_distribution.png
│   ├── revenue_by_date.png
│   ├── top_products_quantity.png
│   └── top_products_revenue.png
```

---

## Future Improvements

* Build an interactive Power BI dashboard.
* Create automated data validation checks.
* Add monthly and weekly sales forecasting.
* Perform customer segmentation analysis.

---

## Author

Nguyen Hong Tien

Aspiring Data Analyst | Python | SQL | Power BI | Excel
