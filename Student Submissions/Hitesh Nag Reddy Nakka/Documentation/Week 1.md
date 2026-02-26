# **Week 1: Power BI Concepts \- Power Query Data Processing**

This document summarizes the key Power Query concepts and data processing steps covered in the first week of instruction. Power Query is a data transformation and preparation engine in Power BI that allows users to connect to, import, and refine data from various sources.

# **Introduction to Power Query**

Power Query Editor is the dedicated window within Power BI where you apply transformations to your data. These steps are recorded and can be re-run whenever the data is refreshed, ensuring consistent data preparation.

# **Key Data Processing Steps**

Below are some fundamental data processing steps explained, which are crucial for cleaning and shaping data before analysis in Power BI.

## **1\. Connecting to Data Sources**

The first step is always to connect to the raw data. Power Query supports a vast number of sources, including:

* **Files:** Excel, CSV, JSON, XML  
* **Databases:** SQL Server, Oracle, MySQL  
* **Online Services:** SharePoint List, Salesforce, Google Analytics

## **2\. Basic Transformations**

Basic transformations are essential for initial data cleanup.

| Transformation | Description | Example Use Case |
| :---- | :---- | :---- |
| **Remove Columns** | Deleting columns that are not needed for analysis. | Removing an internal ID column that is not relevant to reports. |
| **Choose Columns** | Selecting only the required columns, which is a more efficient way to remove unneeded columns. | Picking 'Date', 'Product Name', and 'Sales Amount' from a wide table. |
| **Remove Rows** | Deleting rows based on position (top/bottom) or specific conditions (e.g., duplicates, errors). | Removing the top 5 header rows from an unstructured flat file. |
| **Filter Rows** | Keeping only rows that meet specific criteria. | Filtering a sales table to only include transactions from the year 2025\. |

## **3\. Data Type Handling**

Correct data types are critical for proper calculations and visualizations. Power Query automatically detects types, but manual adjustment is often necessary.

* Ensure columns like dates, numbers, and text are correctly identified.  
* The transformation is accessed via the "Data Type" selector in the column header or the "Transform" tab.

## **4\. Text Transformations**

These steps help standardize and clean up text data.

| Transformation | Description |
| :---- | :---- |
| **Trim** | Removes leading and trailing whitespace from text. |
| **Clean** | Removes non-printable characters. |
| **Case Conversion** | Changes text to Uppercase, Lowercase, or Proper Case. |
| **Split Column** | Divides a single column into multiple columns based on a delimiter (e.g., comma, space). |

