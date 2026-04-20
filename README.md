# 📊 Sales Trend Analysis Using SQL

> 📌 A beginner-friendly SQL project to analyze sales trends using aggregation functions.

---

## 📌 Objective

Analyze **monthly revenue** and **order volume** using SQL aggregation techniques to understand sales trends over time.

---

## 🛠️ Tools Used

* SQLite (DB Browser for SQLite)
* SQL

---

## 🗂️ Dataset

Table: `online_sales`

### Columns:

* `order_id` – Unique ID for each order
* `order_date` – Date of order
* `amount` – Revenue generated
* `product_id` – Product identifier

---

## ⚙️ SQL Concepts Used

* `GROUP BY`
* `SUM()`
* `COUNT(DISTINCT)`
* `ORDER BY`
* `strftime()` (date extraction)

---

## 📈 Analysis Performed

* Extracted **year and month** from order date
* Calculated **monthly revenue**
* Calculated **order volume per month**
* Sorted results in chronological order

---

## 🧾 SQL Query

```sql
SELECT 
    strftime('%Y', order_date) AS year,
    strftime('%m', order_date) AS month,
    SUM(amount) AS total_revenue,
    COUNT(DISTINCT order_id) AS order_volume
FROM online_sales
GROUP BY year, month
ORDER BY year, month;
```

---

## 📊 Results

Final output of the SQL query:

| Year | Month | Total Revenue | Order Volume |
| ---- | ----- | ------------- | ------------ |
| 2024 | 01    | 800           | 2            |
| 2024 | 02    | 900           | 2            |
| 2024 | 03    | 1400          | 2            |
| 2024 | 04    | 1400          | 2            |

---

## 📸 Output

Refer to `output.png` for the query result screenshot.

---

## ✅ Conclusion

This project demonstrates how SQL aggregation functions can be used to analyze sales data and identify trends effectively. It provides a simple yet powerful approach to data analysis using SQL.

---
