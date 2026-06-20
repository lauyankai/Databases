## 1. Project Summary
In this assignment for the SECP2523 Databases course, I focused on the foundational concepts of relational database design, specifically translating real-world business requirements into logical models and Entity-Relationship Diagrams (ERDs). The assignment tested my ability to differentiate between raw data and processed information within an e-commerce context, identifying entities such as Orders, Payments, Products, and Customers.

A major portion of the assignment involved analyzing existing relational schemas (such as a Scientific Experiment database) to identify Primary Keys and Foreign Keys. I was tasked with evaluating whether the tables exhibited **Entity Integrity** (ensuring every table has a valid primary key) and **Referential Integrity** (ensuring foreign keys properly link to existing records). 

Furthermore, I gained hands-on practice in database modelling by designing an entire ERD from scratch for a "Luxury Records" system, mapping out the complex relationships between Musicians, Instruments, Albums, and Songs. The assignment also covered the practical application of different relationship cardinality types (One-to-one, One-to-many, Many-to-many) using both **Chen notation** and **Crow’s Foot notation** to visually represent business rules, such as a doctor treating multiple patients.

---

## 2. Reflection

### What I Have Learnt
* I learned that accurately identifying Primary Keys and Foreign Keys is the absolute most critical step in database design, as failing to establish these connections breaks Referential Integrity, leading to orphaned data or system errors. 
* Practicing both Chen and Crow's Foot notations gave me a versatile toolkit for system design. While Chen notation is excellent for high-level conceptual mapping of attributes and entities, I realized that Crow's Foot notation is much cleaner and more practical for representing cardinality in dense, complex relational schemas. 
* A significant improvement would be transitioning to digital database design tools. Utilizing software like Lucidchart, draw.io, or MySQL Workbench to design these schemas would not only produce cleaner diagrams but also allow for the automatic generation of SQL Data Definition Language (DDL) scripts, better mirroring modern industry practices.