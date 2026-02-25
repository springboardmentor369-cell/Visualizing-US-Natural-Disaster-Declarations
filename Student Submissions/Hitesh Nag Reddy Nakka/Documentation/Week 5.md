# **Week 5: Data Modelling and Relational Concepts**

This document summarizes the key concepts discussed in Week 5 regarding data modelling, specifically focusing on Fact Tables, Dimension Tables, and the types of relationships between them.

#Types of Data

**Categorical Data**: Data that represents categories or groups (e.g., Gender, Country, Product Category).

**Numerical Data**: Data represented by numbers that can be measured or counted (e.g., Sales Amount, Age, Quantity).

**Time-Based Data**: Data related to dates and time, used to analyze trends over periods (e.g., Order Date, Month, Year, Timestamp).


# **1\. Introduction to Data modelling**

Data modelling is the process of creating a visual or conceptual representation of either a whole information system or parts of it to communicate connections between data points and structures. It helps in defining business requirements, improving data quality, and structuring the data for efficient storage and retrieval (especially in data warehouses).

The Star Schema is a foundational concept in dimensional modelling, which separates data into two types of tables: Fact Tables and Dimension Tables.

## **Fact Tables**

Fact tables contain the measurements, metrics, or facts of a business process. They are typically large and contain quantitative data that can be aggregated.

**Key Characteristics:**

* **Contain Numerical Data:** They hold measurable values such as sales amount, quantity sold, time taken, or profit.  
* **Foreign Keys:** They contain foreign keys that link them to the associated dimension tables.


## **Dimension Tables**

Dimension tables contain descriptive attributes related to the business process measurements stored in the fact tables. They answer the "who, what, where, when, why, and how" of the facts.

**Key Characteristics:**

* **Contain Descriptive Data:** They hold attributes like product names, customer addresses, store locations, and dates.  
* **Primary Key:** They have a primary key that uniquely identifies each row and is used for linking to the fact table.

# **3\. Types of Relationships**

Relationships define how two tables are logically connected based on common columns (keys). Understanding these relationships is critical for designing efficient databases and queries.

## **1\. One-to-Many (1:N)**

This is the most common relationship in data modelling.

* **Definition:** A single row in Table A can be related to multiple rows in Table B, but a single row in Table B can be related to only one row in Table A.  
* **Example:** One **Customer** (Table A) can place many **Orders** (Table B). The foreign key is placed in the "many" side (the **Orders** table).

## **2\. One-to-One (1:1)**

This relationship is less common and often indicates that the two tables could potentially be merged.

* **Definition:** A single row in Table A can be related to only one row in Table B, and vice-versa.  
* **Example:** A **Student** (Table A) may have exactly one **Passport Detail** (Table B) record stored in a separate table for security reasons.

## **3\. Many-to-One (N:1)**

This is logically the same as One-to-Many, just viewed from the opposite direction.

* **Definition:** Multiple rows in Table A can be related to a single row in Table B.  
* **Example:** Many **Employees** (Table A) work for one **Department** (Table B). The foreign key is placed in the "many" side (the **Employee** table).

## **4\. Many-to-Many (N:N)**

This relationship is avoided in relational database design and is usually resolved into two 1:N relationships using an intermediary **Junction/Bridge Table**.

* **Definition:** A row in Table A can be related to multiple rows in Table B, and a row in Table B can be related to multiple rows in Table A.  
* **Example:** Many **Students** (Table A) can enroll in many **Courses** (Table B).

# **Power BI Model View**

The Model View in Power BI Desktop is the dedicated area for viewing, managing, and creating relationships between tables in your data model. It provides a visual canvas that simplifies the complex structure of a database, making it an essential tool for data modelling and relationship management.
