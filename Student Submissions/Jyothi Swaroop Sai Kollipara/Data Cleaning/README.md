Data Cleaning Process(Using Python)

The data cleaning process was performed to ensure accuracy, consistency, and reliability before analysis and dashboard creation. The following steps were followed:

Missing Value Analysis:
All columns were checked for missing values to assess data quality. It was observed that the incident end date contained missing entries, which were retained since many disasters are ongoing or single-day events, making the absence of an end date valid.

Removal of Non-Analytical Columns:
Identifier columns such as IDs were removed as they do not contribute to analytical insights or trend analysis.

Data Type Validation:
Columns were reviewed and converted to appropriate data types:

Date fields were formatted as date values

Numeric fields were converted to numerical formats

Categorical fields (state, disaster type, request status) were treated as text

Data Consistency Checks:
Column names and values were verified for consistency to avoid aggregation and visualization issues.

Prepared Dataset for Visualization:
After cleaning and validation, the structured dataset was imported into Power BI for modeling, measure creation, and dashboard development.
