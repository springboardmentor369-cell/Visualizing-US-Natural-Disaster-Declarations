# Week 6: Understanding DAX and Calculated Measures in Power BI
Week 6 focused on understanding Data Analysis Expressions (DAX) in Power BI and how calculations are performed using measures. This week was important because it helped me move beyond just creating visuals and start focusing on logic-based analysis, where numbers are calculated dynamically based on the data model.
## Introduction to DAX
We began by understanding what DAX (Data Analysis Expressions) is. DAX is a formula language used in Power BI for data analysis and calculations. It is mainly used to create calculated measures that help derive meaningful insights from data.

I learned that DAX expressions are not simple formulas but calculations that work across the entire data model.
## Creating the First DAX Measure
We then learned how to create a new measure, starting with the simplest DAX function:
* SUM
This helped build confidence and clarity about how DAX works. Starting with basic aggregation made it easier to understand more complex concepts later.
## Why DAX Measures Are Preferred Over Implicit Measures
An important learning was understanding why we should use explicit DAX measures instead of relying on implicit measures (automatic calculations created when fields are dragged into visuals).
### We learned that:
* DAX measures provide more control
* They are reusable across visuals
* They give more accurate and consistent result
## Two Key Rules While Writing DAX
Two very important points were emphasized:
* 1.Always use explicit DAX measures instead of implicit calculations
* 2.Always have a clear question in mind before writing any DAX formula

This helped me understand that DAX is not about writing formulas blindly, but about answering specific business question
## Implicit vs Explicit Functions
We then learned the difference between:
* Implicit functions – automatically created by Power BI
* Explicit functions – manually written DAX formulas
This clarified why professional dashboards rely more on explicit DAX measures.
## Types of Measures Learned
We also understood that there are two types of measures:
* Base Measures: Simple calculations like total sales or total profit
* Composite Measures: Measures created using base measures for advanced analysis
This showed how complex logic can be built step by step.
## Understanding the CALCULATE Function
A major concept introduced was the CALCULATE function. 
We learned that CALCULATE is used to:
* Apply filters on expressions
* Modify filter context
We also understood its basic structure and why it is considered one of the most powerful DAX function.
## CALCULATE vs Slicers
We learned the difference between using CALCULATE and slicers:
* Slicers are user-driven filters
* CALCULATE applies logic-driven filters inside the measure
This helped me understand when to rely on visuals and when to control logic through DAX.
## Understanding Conditional Logic in DAX
Towards the end of the week, we learned conditional logic, including:
* IF statement
* IF–ELSE logic
* Nested IF
This helped in creating measures that return different values based on conditions, which is very useful in real-world analysis.
## Key Learnings from Week 6
* DAX is used for analytical calculations in Power BI
* Measures are dynamic and context-based
* Explicit measures are more powerful than implicit ones
* CALCULATE helps control filter logic
