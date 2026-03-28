# Bookstore Analytics with SQL

A end-to-end SQL project that simulates a bookstore database and performs business analytics — from schema design and data insertion to revenue tracking, customer segmentation, and marketing ROI analysis.

---

## 🗂️ Project Overview

This project demonstrates how SQL can be used to answer real business questions for an online bookstore. It covers database design, data population, and a series of analytical queries organized step by step.

---

## 🛠️ Tech Stack

- **Database:** MySQL
- **Concepts Used:** DDL, DML, Joins, CTEs, Aggregations, Window Logic, Self-Joins

---

## 🗃️ Database Schema

The database `SWEETY` contains four tables:

| Table | Description |
|---|---|
| `Books` | Book catalog with genre, price, and stock |
| `Customers` | Customer info with city and signup date |
| `Orders` | Purchase records linking customers and books |
| `MarketingSpend` | Ad spend per customer |

---

## 📊 Analytics Performed

| Step | Analysis |
|---|---|
| Step 3 | Revenue by book title |
| Step 4 | Low stock alert (stock < 15) |
| Step 5 | RFM analysis — Recency, Frequency, Monetary |
| Step 6 | Marketing ROI per customer |
| Step 7 | Monthly revenue trend |
| Step 8 | Repeat customers (orders > 1) |
| Step 9 | Average order value |
| Step 10 | Book co-purchase patterns |
| Step 11 | Churned customers (no purchase in 365+ days) |

---

## 🚀 How to Run

1. Open your MySQL client (MySQL Workbench, DBeaver, etc.)
2. Create and select the database:
   ```sql
   CREATE DATABASE SWEETY;
   USE SWEETY;
   ```
3. Run the script in order — schema creation → data insertion → analytics queries.

---

## 💡 Key Insights

- **Top Revenue Book:** Identified using `SUM(quantity * price)` grouped by title
- **RFM Segmentation:** Customers ranked by recency, frequency, and monetary value
- **Marketing ROI:** Profit calculated as `total_revenue - marketing_spend`
- **Co-purchase Analysis:** Books frequently bought together using a self-join on Orders
- **Churn Detection:** Customers inactive for more than 365 days flagged for re-engagement

---

## 📁 File Structure

```
bookstore-analytics-sql/
├── bookstore_analytics.sql   ← Full SQL script (schema + data + queries)
└── README.md
```

---

## 👩‍💻 Author

**Sweety**
Passionate about data analytics and turning raw data into business insights.

---

## ⭐ If you found this project helpful, give it a star!
