# 📚 Online Bookstore Database & Analytics Project

A relational database project that models an online bookstore management system. This project demonstrates database schema design, data relationships, and the execution of basic to advanced SQL queries to extract meaningful business insights.

## 📊 Database Schema

The project utilizes a relational schema with three main entities: **Books**, **Customers**, and **Orders**. 

* **Books**: Tracks inventory, pricing, genres, and publication details.
* **Customers**: Stores customer contact details and geographic locations.
* **Orders**: Captures transactional data linking customers to the books they purchased, including quantities and total revenue.

---

## 🛠️ Tech Stack & Concepts Covered
* **SQL Dialect:** PostgreSQL (utilizes `SERIAL`, `NUMERIC`, and `COALESCE`)
* **DDL (Data Definition Language):** Table creation with `PRIMARY KEY`, `FOREIGN KEY` constraints, and `DROP TABLE IF EXISTS` logic.
* **DML & DQL (Data Querying):** * Aggregations (`SUM`, `AVG`, `COUNT`)
    * Table Joins (`INNER JOIN`, `LEFT JOIN`)
    * Grouping and Filtering (`GROUP BY`, `HAVING`, `WHERE`, `BETWEEN`)
    * Data Sorting & Query Optimization (`ORDER BY`, `LIMIT`, `DISTINCT`)

---

## 🔍 Key Business Insights Solved

The SQL scripts answer critical business questions divided into two levels of complexity:

### 1. Basic Operations & Inventory Tracking
* Filtering inventory by specific genres ("Fiction") and historical milestones (published after 1950).
* Geographic customer segmentation (identifying Canadian clients).
* Time-series sales filtering (tracking orders specific to November 2023).
* Inventory health audits (identifying total stock volume and critical restock levels/lowest stock).

### 2. Advanced Business Intelligence
* **Sales Performance:** Calculating total revenue and breakdown of books sold per genre and per author.
* **Customer Lifetime Value (CLV):** Pinpointing high-value customers (who spent the most) and identifying loyal customers with multiple orders.
* **Inventory Reconciliation:** Dynamically calculating remaining stock by subtracting ordered quantities from initial stock using `COALESCE` to handle unsold books safely.

---

## 🚀 How to Run This Project

### Prerequisites
You will need a SQL database client or environment installed, such as:
* PostgreSQL / pgAdmin
* DBeaver
* An online SQL compiler (e.g., DB Fiddle)
