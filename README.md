# 📊 Sales Trend Analysis Using SQL

## 📌 Objective

Analyze **monthly revenue** and **order volume** using SQL aggregation techniques.

---

## 🛠️ Tools Used

* SQLite (DB Browser for SQLite)
* SQL

---

## 🗂️ Dataset

Table: `online_sales`

**Columns:**

* `order_id` – Unique ID for each order
* `order_date` – Date of order
* `amount` – Revenue generated
* `product_id` – Product identifier

---

## ⚙️ SQL Concepts Used

* GROUP BY
* SUM()
* COUNT(DISTINCT)
* ORDER BY
* strftime()

---

## 📈 Analysis Performed

* Extracted year and month from order date
* Calculated monthly revenue
* Calculated order volume per month
* Sorted results chronologically

---

## 📊 Results

| Year | Month | Total Revenue | Order Volume |
| ---- | ----- | ------------- | ------------ |
| 2024 | 01    | 800           | 2            |
| 2024 | 02    | 900           | 2            |
| 2024 | 03    | 1400          | 2            |
| 2024 | 04    | 1400          | 2            |

---

## 📸 Output

See `output.png` for the query result screenshot.

---

## ✅ Conclusion

SQL aggregation functions help analyze sales trends efficiently and provide meaningful business insights.
