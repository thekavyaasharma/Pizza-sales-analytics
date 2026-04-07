# 🍕 Pizza Sales Analytics — SQL-Driven Data Analysis

![SQL](https://img.shields.io/badge/SQL-MySQL-blue?style=flat-square&logo=mysql&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat-square)
![Level](https://img.shields.io/badge/Level-Beginner--to--Advanced-orange?style=flat-square)

A structured SQL project that explores and analyzes pizza sales data to uncover insights around orders, revenue, customer preferences, and sales trends — spanning beginner to advanced query complexity.

---

## 📌 Table of Contents

- [Project Overview](#project-overview)
- [Database Schema](#database-schema)
- [ER Diagram](#er-diagram)
- [Analysis Levels](#analysis-levels)
  - [Basic](#-basic)
  - [Intermediate](#-intermediate)
  - [Advanced](#-advanced)
- [Dataset Files](#dataset-files)
- [Key Insights](#key-insights)
- [Skills Demonstrated](#skills-demonstrated)
- [Author](#author)

---

## Project Overview

This project performs end-to-end sales analysis on a pizza restaurant dataset using **SQL queries**. It is structured into three analytical tiers — Basic, Intermediate, and Advanced — to progressively explore the data and extract meaningful business insights.

The goal is to answer real-world business questions such as:
- How much total revenue was generated?
- Which pizzas are best-sellers?
- What time of day sees the highest order volume?
- How does revenue accumulate over time?

---

## Database Schema

The project is built on four relational tables:

| Table | Description |
|---|---|
| `pizzas` | Pizza ID, type, size, and price |
| `pizza_types` | Pizza name, category, and ingredients |
| `orders` | Order ID, date, and time |
| `order_details` | Order-level breakdown: pizza ordered and quantity |

---

## ER Diagram

The entity-relationship diagram below illustrates how the four tables are connected:

![ER Diagram](ER%20DIAGRAM.png)

> **Relationships:** `order_details` links `orders` and `pizzas`; `pizzas` links to `pizza_types` via `pizza_type_id`.

---

## Analysis Levels

### 🟢 Basic

Foundational queries to understand the dataset at a high level:

- Total number of orders placed
- Total revenue generated from pizza sales
- Identification of the highest-priced pizza
- Most commonly ordered pizza size
- Top 5 most ordered pizza types by quantity

---

### 🟡 Intermediate

Multi-table joins and aggregations for deeper insight:

- Total quantity ordered per pizza category
- Hourly distribution of orders throughout the day
- Category-wise breakdown of pizza orders
- Average number of pizzas ordered per day
- Top 3 pizza types ranked by total revenue

---

### 🔴 Advanced

Advanced SQL techniques including window functions and subqueries:

- Percentage revenue contribution of each pizza type
- Cumulative revenue over time (running total)
- Top 3 revenue-generating pizzas within each category

---

## Dataset Files

| File | Description |
|---|---|
| `orders.csv` | Order-level data including date and time |
| `order_details.csv` | Line-item breakdown of each order |
| `pizzas.csv` | Pizza sizes and pricing |
| `pizza_types.csv` | Pizza names, categories, and ingredients |
| `sql pizza sales analytics.pdf` | Full SQL query document with results |
| `ER DIAGRAM.png` | Entity-Relationship diagram of the database |

---

## Key Insights

- **Revenue concentration:** A small number of pizza types contribute a disproportionately large share of total revenue.
- **Peak ordering hours:** Orders are heavily concentrated during lunch and dinner hours.
- **Size preference:** Certain pizza sizes consistently dominate across all categories.
- **Category trends:** Classic and Chicken categories tend to outperform others in terms of quantity and revenue.
- **Cumulative growth:** Revenue grows steadily throughout the year with identifiable peak periods.

---

## Skills Demonstrated

- Writing and optimizing SQL queries (SELECT, JOIN, GROUP BY, ORDER BY, HAVING)
- Aggregation functions: `SUM()`, `COUNT()`, `AVG()`, `ROUND()`
- Window functions: `RANK()`, running totals with `SUM() OVER()`
- Subqueries and nested SELECT statements
- Relational database design and ER modeling
- Data analysis and business insight extraction

---

## Author

**Kavya Sharma**
B.Tech CSE (2nd Year)

Feel free to reach out for feedback, collaboration, or discussion!

[![GitHub](https://img.shields.io/badge/GitHub-thekavyaasharma-181717?style=flat-square&logo=github)](https://github.com/thekavyaasharma)
