📊 Week 5 – Visualization Basics (Power BI)

1️⃣ Data Types

Understanding data types is the foundation of visualization and modeling.

Numerical Data
Contains numbers used for calculations.
Examples: Sales amount, Profit, Quantity, Marks.
👉 Used for aggregation like SUM, AVERAGE, COUNT.

String (Categorical) Data
Contains text values used for grouping and labeling.
Examples: Product Name, Region, Customer Name, Department.
👉 Used for comparison across categories.

Time (Date/Time) Data
Contains date-related values.
Examples: Order Date, Year, Month, Quarter.
👉 Used to analyze trends and time-based growth.


2️⃣ Types of Charts & Their Usage

Bar Chart
📌 Used to compare values across categories.
Example: Sales by Product or Region.

Line Chart
📌 Used to show trends over time.
Example: Monthly Revenue Growth.

Pie Chart
📌 Used to show proportion or percentage contribution.
Example: Market Share by Brand.

Column Chart
📌 Similar to bar chart but vertical.
Example: Year-wise Sales Comparison.

Choosing the right chart depends on the type of data and the business question.


3️⃣ Data Modeling

Data modeling helps structure data properly for accurate analysis.

⭐ Star Schema

A commonly used data modeling structure where:

A central Fact Table is connected to multiple Dimension Tables.

It improves performance and simplifies relationships.


4️⃣ Fact Table

Contains numerical and measurable data.

Stores transactional information.

Usually includes foreign keys linking to dimension tables.

Example Columns:
Sales Amount, Quantity, Profit, Order ID.


5️⃣ Dimension Table

Contains descriptive or categorical data.

Provides context to fact table data.

Example Columns:
Product Name, Customer Name, Region, Date.


6️⃣ Types of Relationships (Cardinality)

One-to-One (1:1)
One record in Table A relates to one record in Table B.

One-to-Many (1:N)
One record in a dimension table relates to multiple records in a fact table.
👉 Most common in Star Schema.

Many-to-One (N:1)
Multiple records in one table relate to a single record in another.

Many-to-Many (N:N)
Multiple records in both tables are related.


✅ Summary

In Week 5, we learned:

Different data types and their importance in visualization.

Various charts and their use cases.

Basics of data modeling.

Structure of Star Schema.

Difference between Fact and Dimension tables.

Types of relationships (cardinality) in Power BI.
