# SECP2523: Databases

## 1. Course Overview
Welcome to my GitHub E-Portfolio for the **SECP2523 - Databases** course. This repository showcases my academic progression and practical skills in relational database design, data modelling, and SQL implementation. 

Throughout this course, I developed a strong foundation in translating real-world business requirements into conceptual Entity-Relationship Diagrams (ERDs). I also mastered the process of Database Normalization (from 1NF to 3NF) to eliminate data redundancy and ensure data integrity. The repository concludes with practical, hands-on implementations in MySQL, where I wrote Data Definition Language (DDL) to build physical schemas and advanced Data Manipulation Language (DML) scripts to extract business insights using complex multi-table `JOIN` operations.

## 2. Team Members & Collaborators
While the theoretical assignments were conducted individually, the hands-on MySQL lab activities within this repository were completed collaboratively. I would like to acknowledge my teammates:
*   **Lau Yan Kai (A23CS0098)** 
*   **Chew Chiu Xian (A23CS0061)**
*   **Ahmad Ziyaad Bin Mohd Abbas (A23CS0206)**

---

## 3. Repository Contents (Assignments and Labs)

### 📝 [Assignment 1: Entity Relationship Modelling and Schemas]
*   **Topic:** Conceptual Database Design, Primary/Foreign Keys, and ERDs.
*   **Summary:** Focused on translating business rules into logical models. Analyzed existing schemas (like a Scientific Experiment database) to verify Entity and Referential Integrity. Drew comprehensive ERDs for a "Luxury Records" system using both Chen and Crow’s Foot notations to accurately map relationships between musicians, albums, instruments, and songs.

### 📝 [Assignment 2: Database Normalization]
*   **Topic:** Eliminating Data Redundancy and Update Anomalies (1NF, 2NF, 3NF).
*   **Summary:** Systematically broke down unnormalized, bulky datasets into highly efficient relational tables. Handled two main case studies: transforming a student traffic offences table into First Normal Form (1NF), and executing a complete normalization process (up to 3NF) for a consulting company’s operations to eliminate partial and transitive dependencies.

### 💻 [Lab Activity 1: Creating the Tennis Logos Database]
*   **Topic:** MySQL DDL Implementation and Referential Integrity.
*   **Summary:** Built a foundational relational database named `TL_Sport` for a fictional customized clothing company. Utilized SQL Data Definition Language (DDL) to create `Supplier` and `Item` tables, securing them with Foreign Key constraints. Practiced Data Manipulation Language (DML) by executing `INSERT INTO` statements to populate inventory data, and performed safe database teardown by dropping constraints before tables.

### 🔍 [Lab Activity 2: SQL Data Manipulation and Queries]
*   **Topic:** Advanced Data Extraction, Multi-Table JOINs, and Aggregations.
*   **Summary:** Extracted meaningful business intelligence from a simulated online bookstore database containing `books`, `customers`, `orders`, and `order_items` tables. Wrote 15 complex SQL scripts utilizing `INNER JOIN` and `LEFT JOIN` date filtering like `CURDATE()`, and advanced aggregations using `GROUP BY`, `HAVING`, `SUM()`, `AVG()`, and `COUNT()` to identify high-value customers and calculate total store revenue.