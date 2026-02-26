🧹 Data Cleaning Using Power BI

Data cleaning was performed in Power BI to prepare the dataset for accurate analysis and visualization. The following steps were carried out:

Imported the raw FEMA disaster declaration dataset into Power BI Desktop.

Reviewed all columns to understand their purpose, relevance, and structure.

Analyzed missing values using Power BI’s data profiling tools.

Identified missing values in the incident end date column and retained them, as many disasters are ongoing or single-day events where an end date may not be available.

Removed non-analytical identifier columns that do not contribute to insights or trend analysis.

Verified and corrected data types:

Date-related fields were formatted as date values

Numeric fields were set as numerical types

Categorical fields such as state and disaster type were treated as text

Ensured column naming consistency to improve readability and usability.

Validated data integrity to avoid aggregation and visualization errors.

After these steps, the dataset was clean, structured, and ready for exploratory analysis and dashboard creation.

📊 Dashboard Development Using Power BI

An interactive dashboard solution was developed in Power BI to analyze disaster declaration trends and patterns effectively. The dashboard creation process included the following steps:

Loaded the cleaned dataset into Power BI Desktop.

Created calculated columns and DAX measures to support analysis.

Defined key KPIs such as:

Total Requests – overall number of disaster declaration requests

Unique States – number of states affected

Designed KPI cards to present high-level insights at a glance.

Built visualizations based on business-driven questions:

Bar charts to analyze top disaster types and state-wise request distribution

Line chart to observe year-wise disaster trends

Geographic map to visualize state-wise concentration of disaster requests

Added interactive slicers for:

State

Disaster Type

Year
enabling dynamic filtering across all visuals.

Applied professional formatting, alignment, and background styling to enhance readability and presentation.

Ensured all visuals and KPIs respond correctly to slicer selections.

The final dashboard provides an end-to-end analytical view of disaster declaration data, enabling interactive and data-driven exploration.

🆕 📅 Today’s Work – Post Data Cleaning & Dashboard Refinement

After completing data cleaning, today’s work focused on transforming cleaned data into decision-ready dashboards and refining them through review and improvement.

🔹 Dashboard Structuring Based on Questions

Designed separate dashboards for separate business questions instead of combining all insights into one view.

Ensured each dashboard answers one clear analytical question.

🔹 KPI & Measure Enhancement

Created advanced DAX measures to calculate:

High-Risk States (states above national average)

Peak Year and Peak Year Declarations

Average Annual Declarations

Validated all KPIs for accuracy and correct filter behavior.

🔹 Dashboard Review & Optimization

Reviewed visuals to confirm they support the intended question.

Removed unnecessary or redundant charts.

Improved visual hierarchy using a top-down structure:

KPIs at the top

Trends and comparisons in the middle

Supporting visuals at the bottom

🔹 Color & Design Improvements

Applied consistent color logic:

Red for high risk / extreme values

Blue for normal or neutral values

Updated dashboard background to neutral tones for better readability.

Added card backgrounds and subtle shadows for a professional appearance.

🔹 Validation & Final Checks

Verified that all visuals respond correctly to slicers.

Ensured dashboard insights are easy to interpret within a few seconds.

Confirmed that dashboards are suitable for presentation to mentors, reviewers, or stakeholders.

✅ Outcome of Today’s Work

Cleaned data successfully converted into two purpose-driven dashboards

Dashboards refined to be clear, professional, and decision-focused

Project now reflects an end-to-end analytics workflow, from raw data to actionable insights
