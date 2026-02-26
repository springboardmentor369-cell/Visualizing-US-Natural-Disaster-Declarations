# Week 5: Visualizations and Data Modeling in Power BI
Week 5 focused on understanding how cleaned and analyzed data is transformed into meaningful visualizations that support effective decision-making. I learned that building impactful dashboards is not only about visual design, but also about understanding the nature of the data and structuring it correctly through data modeling before creating visuals.
## Different Dataset Types
The Types of datasets, play a crucial role in selecting appropriate visualizations:
1. Numerical Data {Number}
Data that can be measured or calculated, such as sales, revenue, profit, quantity, or call duration.
2. Categorical Data {Nominal}
Data that represents categories or groups, such as product type, region, customer segment, or department.
3. Time-Based Data
Data related to time intervals, such as dates, days, months, quarters, or years.
- Understanding these dataset types helped me realize that choosing the wrong visualization can mislead users or cause misinterpretation of insights.

## Importance of Visualizations
This week highlighted the role of visualizations in Power BI. Visuals convert complex datasets into clear and actionable insights. I learned that effective visualizations:
* Reveal trends and patterns
* Make comparisons easy and intuitive
* Communicate insights quickly
* Support faster and better business decisions

## The differnt Types Of Charts/Graphs
### Bar Chart
Bar charts are best suited for comparing values across different categories. They are simple, clear, and highly effective for side-by-side comparisons.
### Pie Chart
Pie charts represent proportions or percentage distribution of a whole. I learned that they should be used only when there are limited categories, as too many slices can reduce clarity.
### Line Chart
Line charts are primarily used for time-based data. They help in understanding trends, growth, or decline over a period of time.

## Introduction to Data Modeling
After learning about visualizations, we were introduced to data modeling, which is essential when working with multiple or large datasets. Data modeling defines how tables are connected in Power BI. Without proper modeling, reports may produce incorrect calculations and misleading insights.

## Keys in Data Modeling
We learned about different types of keys used in databases:
### Primary Key
Uniquely identifies each record in a table.
### Foreign Key (Secondary Key)
Used to create relationships between tables.
- Understanding keys helped me see how data flows between tables in Power BI.
 
## Relationships and there Types
We learned that relationships are critical in data modeling to ensure accurate analysis. 
Relationships define how tables are connected using keys.
The different types of relationships include:
### 1. One-to-One (1:1)
* One record in Table A relates to one record in Table B
* Rarely used
Example: Person ↔ Passport
### 2. One-to-Many (1:M)
* One record in Table A relates to many records in Table B
* Most common relationship
Example: One customer → many orders
### 3. Many-to-One (M:1)
* Many records in Table A relate to one record in Table B
* Reverse of one-to-many
Example: Many sales → one product
### 4. Many-to-Many (M:M)
* Many records in both tables match
* Requires a bridge table
Example: Students ↔ Courses
- Choosing the correct relationship type ensures correct aggregations and reliable dashboard results.

## Fact Table and Dimension Table
- This structure helps organize large datasets efficiently.
- Understanding Relationships Between Tables
The difference Are:
### Fact Table
* Contains numerical and measurable data such as sales amount, profit, or quantity.
* Usually large in size.
### Dimension Table
* Contains descriptive data such as customer details, product information, or dates.
* Usually smaller and used for filtering and grouping.

## Star Schema
we learned about the Star Schema, a widely used data modeling approach in Power BI. In this structure:
* The fact table is placed at the center
* Dimension tables are connected around it

### Importance of star schema:
* Improves report performance
* Simplifies data relationships
* Enhances clarity and accuracy of analysis

## Key Learnings from Week 5
* Understanding dataset types is essential before creating visualizations
* Different visuals communicate data in different ways
* Data modeling forms the foundation of accurate dashboards
* Fact and dimension tables help structure large datasets
* Proper relationships and star schema improve performance and reliability
