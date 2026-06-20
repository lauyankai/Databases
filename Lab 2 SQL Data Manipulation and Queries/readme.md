## 1. Project Summary
In this lab activity for the SECP2523 Databases course, my team and I focused on practical **SQL Data Manipulation Language (DML)** by querying a simulated relational database for an online bookstore. The database schema consisted of four interconnected tables: `books`, `customers`, `orders`, and `order_items`. 

The core objective was to extract meaningful business insights by writing 15 complex SQL queries. The lab progressed from basic data retrieval to highly advanced operations. Key SQL concepts mastered during this activity include:
*   **Basic Filtering & Date Operations:** Utilizing the `WHERE` clause and date functions (like `CURDATE() - INTERVAL 30 DAY`) to find recently registered customers and recent orders.
*   **Multi-Table `JOIN` Operations:** Writing `INNER JOIN` and `LEFT JOIN` statements to link up to four tables simultaneously (e.g., tracking a customer's details to their specific book orders).
*   **Data Aggregation (`GROUP BY` & `HAVING`):** Utilizing aggregate functions like `SUM()`, `COUNT()`, `AVG()`, and `MAX()` to calculate total store revenue, average book prices by genre, and total orders per customer. We also applied the `HAVING` clause to filter grouped data, such as finding customers who spent more than $500.
*   **Sorting & Limiting:** Using `ORDER BY ... DESC` and `LIMIT` to identify top-performing metrics, such as the top 5 customers with the most orders or the single most popular book genre.
*   **Subqueries & Null Checks:** Finding customers who had *never* placed an order using `LEFT JOIN` combined with `IS NULL`, and utilizing subqueries to find the most expensive book in the store.

---

## 2. Reflection

### What I Have Learnt

* Before this lab, I understood how tables were connected via Foreign Keys, but writing multi-table `JOIN` statements showed me exactly *how* that connected data is pulled together to answer real business questions. 
* I gained a deep appreciation for the power of SQL aggregate functions. Calculating the total revenue of the entire bookstore by multiplying `books.price` by `order_items.quantity` across a `JOIN` operation demonstrated how raw database records are transformed into actionable Business Intelligence (BI).
* This lab would be vastly improved by executing these queries in a live, populated Relational Database Management System (RDBMS) like MySQL Workbench or DBeaver. Running the queries against thousands of mock records would allow students to see the actual output tables and learn how to read SQL execution plans, which is a critical skill for optimizing slow queries in the real world.