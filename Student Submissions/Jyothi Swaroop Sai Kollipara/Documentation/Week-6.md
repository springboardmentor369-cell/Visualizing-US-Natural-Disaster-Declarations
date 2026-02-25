📘 Week 6 – DAX Functions (Power BI)

This week, our complete focus was on DAX (Data Analysis Expressions) — the formula language used in Power BI to perform calculations and create dynamic insights.


🔹 1️⃣ Basics of DAX

DAX is used to:

Create calculated columns

Create measures

Apply filters

Perform conditional logic

Modify filter context

📌 Basic DAX Syntax
Measure Name = FUNCTION(Column)

✅ Example:
Total Sales = SUM(Sales[SalesAmount])


This measure calculates the total of the SalesAmount column.

🔹 2️⃣ Why We Use DAX

We use DAX to:

Perform dynamic calculations

Create business KPIs

Apply filters within formulas

Generate insights based on slicers and visuals

Without DAX, Power BI would only show basic aggregations.


🔹 3️⃣ Sigma (∑) Symbol Concept

When a column contains the sigma (∑) symbol, it means:

It is a numeric column

It can be aggregated (SUM, AVERAGE, COUNT, etc.)

It can be directly used inside DAX formulas

Example:

If SalesAmount has ∑, we can write:

Average Sales = AVERAGE(Sales[SalesAmount])


Columns without ∑ (like Product Name) are categorical and cannot be directly summed.


🔹 4️⃣ Types of DAX
🟢 Implicit DAX

Automatically created by Power BI

Happens when you drag a numeric (∑) column into a visual

Example: Dragging SalesAmount automatically applies SUM

✔ Easy to use
❌ Limited customization


🔵 Explicit DAX

Manually written using DAX formulas

Provides full control over filter context and logic

Example:

Profit Margin = DIVIDE(SUM(Sales[Profit]), SUM(Sales[SalesAmount]))


✔ Flexible
✔ Custom logic
✔ Professional approach


🔹 5️⃣ Measures in DAX
🟣 Base Measure

Simple calculation created directly from a numeric column.

Example:

Total Profit = SUM(Sales[Profit])

🟠 Composite Measure

Created using one or more existing measures.

Example:

Profit Percentage = DIVIDE([Total Profit], [Total Sales])


Composite measures improve reusability and clean model structure.


🔹 6️⃣ CALCULATE Function

The CALCULATE() function is one of the most powerful DAX functions.

It modifies the filter context of a calculation.

Syntax:
CALCULATE(Expression, Filter)

Example:
Sales in 2024 = CALCULATE(
    SUM(Sales[SalesAmount]),
    Sales[Year] = 2024
)


This calculates total sales only for the year 2024.


🔹 7️⃣ Conditional Logic in DAX

DAX allows logical conditions using IF, AND, OR.

Example:
Performance Status =
IF([Total Sales] > 100000,
   "High Performance",
   "Needs Improvement"
)


This creates a label based on sales value.


✅ Week 6 Summary

In Week 6, we learned:

Basics of DAX and its syntax

Importance of sigma (∑) numeric columns

Difference between Implicit and Explicit DAX

Creation of Base and Composite measures

Use of the powerful CALCULATE() function

Application of Conditional Logic

This week helped us understand how to create dynamic, filter-based, and logic-driven calculations in Power BI using DAX.
