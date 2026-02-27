
# Data Cleaning in Python (Pandas)

## 1. Introduction
Data cleaning in Python using the **Pandas library** replicates the workflow from Power BI while adding automation and scalability. The objective is to transform the **FEMA Disaster Declarations dataset** into a clean, standardized format ready for analysis. Python scripts provide flexibility for handling larger datasets and integrating advanced preprocessing steps, making the workflow reproducible and efficient.

## 2. Step-by-Step Procedure

### 2.1 Importing Data
- **Source**: FEMA Disaster Declarations dataset (CSV format).  
- **Code**:
```python
import pandas as pd
df = pd.read_csv("fema_disaster_declarations.csv")
```
- **Outcome**: The dataset loads into a Pandas DataFrame for cleaning and transformation.


### 2.2 Removing Unnecessary Columns
- **To Do**: Drop metadata and unused fields that do not contribute to analysis.  
- **Procedure**:
```python
df = df.drop(columns=[
    "stateCode", "disasterPageUrl", "shapefileUrl",
    "kmzfileUrl", "geoJsonUrl", "id", "hash", "lastRefresh"
])
```
- **Outcome**: Irrelevant fields are removed, reducing clutter and improving performance.


### 2.3 Checking Data Types
- **To Do**: Ensure correct data types for each column.  
- **Procedure**:
```python
df["disasterNumber"] = df["disasterNumber"].astype(int)

date_cols = ["declarationDate", "incidentBeginDate", "incidentEndDate",
             "entryDate", "closeoutDate", "updateDate"]

for col in date_cols:
    df[col] = pd.to_datetime(df[col], errors="coerce")
```
- **Outcome**: Numeric, text, and date fields are standardized for consistent calculations and aggregations.


### 2.4 Handling Missing Values
- **Procedure**:
  - Retain `closeoutDate` as null to indicate ongoing disasters.  
  - Add a derived **status column** to categorize records as `"Closed"` or `"Open"`.  
```python
df["status"] = df["closeoutDate"].apply(
    lambda x: "Closed" if pd.notnull(x) else "Open"
)
```
- **Outcome**: Missing values are handled logically, ensuring completeness without losing meaning.


### 2.5 Creating Derived Columns
Derived fields enrich the dataset for deeper analysis.

- **Fiscal Year**:
```python
df["fyDeclared"] = df["declarationDate"].apply(
    lambda x: x.year + 1 if x.month > 9 else x.year
)
```

- **Incident Duration**:
```python
df["incidentDuration"] = (
    (df["incidentEndDate"] - df["incidentBeginDate"]).dt.days
)
```

- **Assistance Flags**:
```python
flag_cols = ["iaProgramDeclared", "ihProgramDeclared",
             "paProgramDeclared", "hmProgramDeclared"]

for col in flag_cols:
    df[col] = df[col].astype(bool)
```

- **Outcome**: Derived fields such as Fiscal Year, Incident Duration, and Assistance Flags provide richer insights for dashboards.



### 2.6 Removing Duplicates
- **Procedure**:
```python
df = df.drop_duplicates()
```
- **Outcome**: Duplicate records are removed, ensuring unique entries and preventing double counting.



### 2.7 Exporting Cleaned Data
- **Procedure**:
```python
df.to_csv("fema_cleaned.csv", index=False)
```
- **Outcome**: The cleaned dataset is saved as a CSV file, ready for visualization and further analysis.



## 3. Final Outcome
By the end of the cleaning workflow:
- The FEMA dataset is **cleaned, standardized, and structured** using Python (Pandas).  
- Derived fields such as **Fiscal Year, Incident Duration, Assistance Flags, and Status** are created.  
- The workflow is **script-based, scalable, and automated**, making it suitable for larger datasets and repeatable preprocessing tasks.  
