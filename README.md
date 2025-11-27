# 🍕 Pizza Sales Data Analysis Project

## 📌 Overview

This project is an **end-to-end Data Analytics project** based on a Pizza Sales dataset. The goal is to perform **data cleaning, SQL analysis, and create a Power BI dashboard** to generate insights about pizza sales trends, customer behavior, and revenue patterns.

This project showcases:

* SQL for data exploration & analysis
* Excel for data cleaning & validation
* Power BI for creating interactive dashboards
* Insight generation with real business impact

---

## 📂 Project Structure

```
📁 pizza-sales-analysis
│
├── data/                    # Raw & cleaned datasets
├── sql/                     # SQL scripts
├── powerbi/                 # PBIX dashboard file
├── images/                  # Dashboard screenshots
└── README.md                # Documentation
```

---

## 🛠️ Tools & Technologies

* **SQL Server** – Data querying & analysis
* **Excel** – Data cleaning, formatting
* **Power BI** – Dashboard & visualization
* **GitHub** – Version control

---

## 🧹 1. Data Cleaning (Excel)

Steps performed:

* Removed null and duplicate rows
* Corrected data types (dates, prices, integers)
* Standardized pizza names and categories
* Fixed inconsistent time formats

---

## 🧠 2. SQL Analysis (SQL Server)

### Key Questions Answered:

* Total revenue generated
* Total number of orders
* Most sold pizza type
* Most profitable pizza category
* Peak order times
* Sales by pizza size (S, M, L, XL)
* Revenue per order

### Example SQL Queries

#### ✔ Total Revenue

```sql
SELECT SUM(total_price) AS total_revenue
FROM pizza_sales;
```

#### ✔ Total Orders

```sql
SELECT COUNT(DISTINCT order_id) AS total_orders
FROM pizza_sales;
```

#### ✔ Top 5 Best-Selling Pizzas

```sql
SELECT TOP 5 pizza_name, SUM(quantity) AS total_sold
FROM pizza_sales
GROUP BY pizza_name
ORDER BY total_sold DESC;
```

#### ✔ Revenue by Category

```sql
SELECT pizza_category, SUM(total_price) AS revenue
FROM pizza_sales
GROUP BY pizza_category;
```

---

## 📊 3. Power BI Dashboard

Key visuals included:

* **KPI cards**: Total Revenue, Total Orders, Average Order Value
* **Bar charts**: Top 5 pizzas by revenue & quantity
* **Pie charts**: Sales share by pizza category
* **Area chart**: Daily & monthly sales trend
* **Matrix table**: Sales by pizza size
* **Slicers**: Category, date, size

---

## 🧩 Insights & Findings

### 🔥 Major Insights

* Large-sized pizzas contribute the highest revenue.
* Dinner time (6 PM – 9 PM) has the highest number of orders.
* Supreme & Classic categories dominate total sales.
* Weekends show significantly higher order volume.
* A few pizzas contribute disproportionately to total revenue (Pareto principle).

### 💡 Business Recommendations

* Increase staffing during evening hours.
* Promote high-margin pizzas.
* Offer weekend combo deals.
* Provide discounts on low-selling pizzas to boost engagement.

---

## 📎 Files Included

* `pizza_sales.sql` – All SQL queries
* `dashboard.pbix` – Power BI dashboard
* `cleaned_pizza_sales.xlsx` – Clean dataset
* `README.md` – Documentation

---

## 🚀 How to Run This Project

1. Import the dataset into SQL Server
2. Run SQL queries from the `sql/` folder
3. Load cleaned dataset into Power BI
4. Refresh visuals & interact with dashboard

---

📬 Contact

Manoj Kumar Toppo
GitHub: manoj-toppo
Email: manoj5kumar805@gmail.com

