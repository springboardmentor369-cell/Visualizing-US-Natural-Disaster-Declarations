## Week 6: Understanding DAX and Calculated Measures in Power BI

Week 6 is mainly based on **Data Analysis Expressions (DAX)** and understanding how **calculated measures** work in Power BI. This week was a major shift from only creating visuals to performing **logic-driven, dynamic analysis**, where results change automatically based on filters, slicers, and the data model.

---

## Introduction to DAX

DAX (Data Analysis Expressions) is a **formula language** used in Power BI to perform calculations and data analysis. It is primarily used to create **measures**, **calculated columns**, and **tables**, though the main focus this week was on measures.
DAX functions play a crucial role in Power BI by enabling advanced calculations, dynamic filtering, and time-based analysis. Understanding DAX concepts like CALCULATE, context, measures, and time intelligence helps create meaningful and interactive reports for effective decision-making.

* DAX works on the **entire data model**, not just a single cell
* Calculations are evaluated based on **filter context**
* DAX is designed to answer **business questions**, not just perform math

## Key Components of DAX
### DAX Syntax
* DAX formulas start with an equals (=) sign
* Case-insensitive
* Uses functions, operators, and references
   * Example: Total Sales = SUM(Sales[Amount])

---

## Creating the First DAX Measure

We began by creating a basic measure using simple aggregation functions such as:

* `SUM()`
* `COUNT()`
* `AVERAGE()`

Starting with `SUM()` helped build clarity and confidence in writing DAX. It showed how measures are evaluated dynamically depending on filters applied through visuals or slicers.

---

## Why DAX Measures Are Preferred Over Implicit Measures

An important concept was understanding the limitations of **implicit measures** (auto-generated calculations when dragging fields into visuals) and why **explicit DAX measures** are preferred.

### Advantages of Explicit Measures:

* Full control over logic
* Reusable across multiple visuals
* Consistent and accurate results
* Easier to maintain and optimize
* Industry-standard practice for professional dashboards

---

## Two Key Rules While Writing DAX

Two important rules were emphasized while working with DAX:

1. Always create **explicit DAX measures** instead of relying on implicit calculations
2. Always start with a **clear business question** before writing any DAX formula

This reinforced the idea that DAX is about **problem-solving and analysis**, not random formula writing.

---

## Implicit vs Explicit Functions

We clearly differentiated between:

* **Implicit functions**: Automatically created by Power BI when fields are added to visuals
* **Explicit functions**: Manually written DAX measures with defined logic

Professional and scalable dashboards rely heavily on **explicit DAX measures** for better control and performance.

---

## Types of Measures Learned

We learned that measures can be categorized into two types:

### 1. Base Measures

* Simple aggregations
* Examples: Total Sales, Total Profit, Total Quantity

### 2. Composite Measures

* Built using base measures
* Used for advanced metrics such as profit margin, growth percentage, and KPIs

This step-by-step approach showed how complex analysis can be built logically from simple measures.

---

## Understanding Filter Context and Row Context

A key theoretical concept introduced was **context** in DAX:

* **Filter Context**: Filters applied through slicers, visuals, or DAX expressions
* **Row Context**: Calculations performed row by row (mainly in calculated columns)

Understanding context is essential to writing correct and efficient DAX measures.

---

## Understanding the CALCULATE Function

One of the most important DAX functions introduced was **`CALCULATE()`**. We learned that CALCULATE is used to:

* Modify filter context
* Apply logic-based filters inside a measure
* Re-evaluate expressions under new conditions

Basic structure:

```
CALCULATE(Expression, Filter1, Filter2, ...)
```

CALCULATE is considered the **core function of DAX** because many advanced calculations depend on it.

---

## CALCULATE vs Slicers

We compared the use of CALCULATE with slicers:

* **Slicers**: User-driven, interactive filters
* **CALCULATE**: Logic-driven, controlled inside the measure

This distinction helped understand when to allow users to control data and when logic should be enforced through DAX.

---

## Conditional Logic in DAX

Towards the end of the week, we learned **conditional logic**, which is essential for real-world business scenarios.

Concepts covered:

* `IF()` statement
* IF–ELSE logic
* Nested IF conditions

These are useful for:

* Performance classification
* Status indicators
* Threshold-based calculations

---

## Introduction to Time Intelligence (Overview)

We were briefly introduced to **time-based analysis**, which uses DAX functions to analyze data over time, such as:

* Year-to-Date (YTD)
* Month-over-Month (MoM)
* Year-over-Year (YoY)

This highlighted how powerful DAX can be when working with date tables.

---

## Key Learnings from Week 6

* DAX is used for advanced analytical calculations in Power BI
* Measures are dynamic and respond to filter context
* Explicit measures are more powerful and professional than implicit ones
* CALCULATE plays a central role in controlling logic and filters
* Understanding context is critical for correct DAX results
* Conditional logic enables decision-based metrics

