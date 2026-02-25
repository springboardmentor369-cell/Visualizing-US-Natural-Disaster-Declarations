# **Week 3: Exploratory Data Analysis (EDA) using Python**

This document summarizes the key steps for Exploratory Data Analysis (EDA) using the **Python Pandas library** within a **Jupyter Notebook environment** hosted in **VS Code** and how important to understand the business behind the data.

EDA is a critical step in the data science process, allowing us to understand the dataset's main characteristics, discover patterns, spot anomalies, and prepare the data for modeling.

# **1\. Environment and Setup**

The session utilized the following tools:

* **Python:** The core programming language.  
* **Jupyter Notebook:** An interactive computing environment used for running code, visualizing data, and documenting analysis.  
* **VS Code (Visual Studio Code):** The code editor/IDE used to host and run the Jupyter Notebook.

# **2\. Importing Data into Python (Pandas)**

The first step in any analysis is loading the data into a Pandas DataFrame.pd.read\_excel("data\_file.xlsx")

The `pd.read_excel()` function is used to load data from an Excel file into a Pandas DataFrame, where `pd` is the standard alias for the Pandas library.

# **3\. Key Data Cleaning and Preprocessing Steps**

The following are the essential data cleaning operations demonstrated to ensure data quality and integrity, paralleling some of the preparation steps done in Power Query.

## **Removing Duplicates**

This command identifies and removes all duplicate rows from the DataFrame, keeping the first occurrence.df \= df.drop\_duplicates()

## **Text Data Cleaning (Last Name Example)**

Standardizing text fields is crucial for accurate analysis. These commands focus on cleaning the `Last_Name` column.

### **Removing Leading and Trailing Whitespace**

The `.str.strip()` method removes any unwanted spaces from the beginning or end of the text strings in the column.df\["Last\_Name"\] \= df\["Last\_Name"\].str.strip()

### **Removing Specific Unwanted Characters**

The `.str.strip()` method can also remove specified leading/trailing characters (e.g., slashes, periods, or underscores) from the text strings.df\["Last\_Name"\] \= df\["Last\_Name"\].str.strip("/.\_")

### **Global Text Replacement**

The `.str.replace()` method is used to substitute specific substrings with new values across a text column.

## **Removing Unnecessary Columns**

To streamline the dataset and focus on relevant variables, columns not needed for analysis are dropped.df \= df.drop(columns=\["Not\_Useful\_Column"\])

## **Understanding Business Context Before Analysis**

Before starting EDA, it is important to understand the business behind the data. In the case of Netflix, the dataset represents its content library, which directly affects:

* Subscriber growth  
* Viewer engagement  
* Content investment decisions  
* Regional market expansion

Thinking from a business perspective means analyzing data with the intention of answering real-world business needs.

Each step helps transform raw data into actionable business understanding.

* **Initially check the volume of data**  
   This step helps understand the size of the dataset by identifying the number of rows and columns, which gives an idea about the scale and complexity of the data.

* **Understanding how diverse the dataset is**  
   This step focuses on identifying variety in the data such as different categories, genres, countries, or types, showing how well the dataset represents multiple segments.

* **Comparison of categories**  
   This step involves comparing different categories to find dominant, popular, or underperforming groups within the dataset.

* **Relationships of data**  
   This step helps identify patterns and associations between different variables in the dataset to understand how one factor influences another.

