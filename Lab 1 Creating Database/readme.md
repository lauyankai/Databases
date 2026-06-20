## 1. Project Summary
In this lab activity for the SECP2523 Databases course, my team and I transitioned from theoretical database design to practical implementation using **MySQL**. The objective was to build a foundational relational database named `TL_Sport` for a fictional customized clothing company called "Tennis Logos". 

We utilized SQL **Data Definition Language (DDL)** to create the physical schema. This involved creating a `Supplier` table with a Primary Key (`SupplierCode`), and an `Item` table that securely linked back to the supplier using a Foreign Key constraint. 

Following the table creation, we utilized SQL **Data Manipulation Language (DML)**. We wrote `INSERT INTO` statements to populate the tables with wholesale pricing and inventory data, and executed `SELECT *` queries to retrieve and verify the structured information. Finally, we practiced safe database teardown procedures by successfully dropping the foreign key constraints before dropping the tables themselves.

## 2. Reflection

### What I Have Learnt

* I learned the importance of execution order in relational databases. Because the `Item` table relies on the `Supplier` table for its Foreign Key, I learned that the `Supplier` table *must* be created and populated first. 
* When destroying the database, the child constraints must be dropped before the parent tables can be deleted. Understanding these strict relational dependencies is crucial for preventing fatal database errors.
* A highly beneficial improvement would be to introduce **SQL JOIN** operations in this phase. Since the data is split between the `Supplier` and `Item` tables, writing a query that joins the two tables together to display the "Item Description" alongside the full "Supplier Name" would provide a much more realistic view of how businesses actually extract value from relational schemas.