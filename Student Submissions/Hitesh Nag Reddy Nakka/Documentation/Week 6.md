# **Week 6 – DAX Functions and Calculations in Power BI**

# **Introduction to DAX**

DAX (Data Analysis Expressions) is the brain of Power BI used to perform powerful calculations and data analysis. It allows us to create custom measures, apply filters, implement conditional logic, and gain deeper insights from data.

## **Key Points Learned**

* DAX is used to create calculations that cannot be achieved through basic visualization.  
* Measures provide better control over aggregation and formatting.  
* Measures are not stored as physical columns; they are calculated dynamically based on the visual context.  
* The Sigma (∑) symbol represents measures, while the table icon represents columns.  
* Auto formatting can remove unnecessary decimals for better readability.  
* Explicit DAX measures are preferred over implicit measures because they are reusable and provide more flexibility.  
* DAX helps answer business questions by creating meaningful metrics.

# **Types of Measures**

## **Base Measures**

Base measures are fundamental calculations created directly from columns. They serve as building blocks for more complex measures.

**Example:** `Total Revenue = SUM(FactSales[Revenue])`

## **Composite Measures**

Composite measures are created using existing base measures.

**Example:** `Total Revenue = [Total Cost] + [Total Profit]`

## **Why use them?**

* Reduce repetition  
* Improve readability  
* Make the data model scalable

# **CALCULATE Function**

The `CALCULATE` function is one of the most powerful functions in DAX. It modifies the filter context to return specific results.

## **Important Concepts**

* Used to apply filters on expressions.  
* More specific than slicers because it controls calculations at the formula level.  
* Slicers affect the entire dashboard, while `CALCULATE` can target a particular measure.  
* Helps in answering targeted business questions.

# **Implemented DAX Measures**

## **1\. Total Profit**

`Total Profit = SUM(FactSales[Profit])`

| How it works: | Adds all values from the Profit column. Returns the aggregated profit based on the current filter context. |
| :---- | :---- |
| **Why used:** | Acts as a base measure. Helps analyze profitability across employees, regions, or products. |

## **2\. Profits from Managers**

`Profits from managers = CALCULATE([Total Profit], DimEmployee[Role] = "Manager")`

| How it works: | Uses CALCULATE to filter employees whose role is Manager. Computes profit only for that group. |
| :---- | :---- |
| **Why used:** | Enables role-based performance analysis. Helps management evaluate contribution from leadership staff. |

## **3\. Sales Target (Conditional Logic)**

`Sales target = IF([Total Profit] > 50000, "Passed", "Failed")`

| **How it works:** | Checks whether total profit exceeds 50,000. Returns Passed if true, otherwise Failed. |
| :---- | :---- |
| **Why used:** | Implements business rules directly in the model. Quickly identifies high-performing employees. |

# **Best Practices Learned**

* Frame business questions before writing DAX.  
* Ensure all relationships are correctly established.  
* Prefer explicit measures for better optimization.  
* Use base measures to build composite measures.  
* Apply conditional logic to generate actionable insights.

