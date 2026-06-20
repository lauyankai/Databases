## 1. Project Summary
In this assignment for the SECP2523 Databases course, I focused entirely on the critical concept of **Database Normalization**. The objective was to understand how to eliminate data redundancy and prevent update anomalies by structuring relational tables according to normal forms.

The assignment consisted of two main problem sets:
*   **Question 1 (STUDENTFINE Table):** I analyzed an unnormalized table recording traffic offences by students. I identified that the table was unnormalized because certain cells contained multiple values (e.g., multiple receipt numbers and dates for a single student). I then transformed this data into **First Normal Form (1NF)**, ensuring each column contained atomic values and defining `StudentID` as the primary key.
*   **Question 2 (Consulting Company Operations):** This task involved a complete normalization process, from an unnormalized state through to **Third Normal Form (3NF)**. I took a bulky table containing project details, employee records, and hourly rates, and systematically broke it down. 
    *   In **1NF**, I established the composite primary keys (`Project number` and `Employee number`). 
    *   In **2NF**, I eliminated partial dependencies by separating the data into dedicated Project and Employee tables. 
    *   Finally, in **3NF**, I removed transitive dependencies by creating a separate table for `Rate category` and `Hourly rate`, ensuring that non-key attributes did not depend on other non-key attributes.

---

## 2. Reflection

### What I Have Learnt
* Before this, I viewed databases similar to Excel spreadsheets, where throwing all information into one massive table seemed "easier" to read. However, manually performing the 1NF, 2NF, and 3NF transformations showed me exactly how much data is duplicated in an unnormalized system. I learned that normalization is essential for maintaining data integrity. 
* By separating the `Rate category` and `Hourly rate` into their own table in 3NF, I ensured that if the company updates a rate, they only have to update it in one single row, rather than across hundreds of employee records. 
* A highly beneficial improvement would be pairing this theoretical exercise with practical SQL application. After designing the 3NF tables, writing the actual `CREATE TABLE` and `INSERT` SQL scripts in a system like MySQL to physically build the normalized relationships (using `FOREIGN KEY` constraints) would bridge the gap between theory and software engineering.