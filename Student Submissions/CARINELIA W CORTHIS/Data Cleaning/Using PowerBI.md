#  Data Cleaning in Power BI – Detailed Guide

## 1. Introduction
Data cleaning is the **foundation of reliable dashboards**. Without it, dashboards risk showing misleading insights due to inconsistencies, duplicates, or missing values. In Power BI, the **FEMA Disaster Declarations dataset** is imported and transformed using **Power Query**. The goal is to:
- Ensure **consistency** in data types and formats.  
- Remove **duplicates and irrelevant fields**.  
- Handle **missing values** logically.  
- Create **derived columns** for richer analysis.  

This cleaned dataset becomes the backbone for accurate dashboards.


## 2. Step-by-Step Procedure

### 2.1 Importing Data
- **Source**: FEMA Disaster Declarations dataset (CSV/Excel format).  
  Download link: [FEMA Disaster Declarations v1](https://www.fema.gov/openfema-data-page/fema-web-disaster-declarations-v1)

- **Process**:
  1. Open **Power BI Desktop**.  
  2. Go to **Home → Get Data**.  
  3. Select the file format (text/CSV).  
  4. Load the dataset into **Power Query Editor** for transformation.  

Note: *Importing through Power Query ensures transformations are applied before loading into the model, keeping raw data intact.*

### 2.2 Removing Unnecessary Columns
- **To Do**: Identify columns irrelevant for analysis (metadata, URLs, technical IDs).  
- **Procedure**:
  - Right-click the column → **Remove**.  
  - Maintain a **log of removed fields** for reproducibility.  

- **Removed Columns**:
  - `stateCode`  
  - `disasterPageUrl`  
  - `shapefileUrl`  
  - `kmzfileUrl`  
  - `geoJsonUrl`  
  - `id`  
  - `hash`  
  - `lastRefresh`  

*Removing clutter reduces dataset size, improves performance, and keeps dashboards focused on meaningful fields.*

### 2.3 Checking Data Types
- **To Do**: Ensure each column has the correct data type.  
- **Procedure**:
  - In Power Query, check column type icons:  
    - **ABC** = Text  
    - **123** = Number  
    - **Calendar** = Date  
  - Adjust where needed:  
    - `disasterNumber` → Whole Number  
    - Date fields (`declarationDate`, `incidentBeginDate`, `incidentEndDate`, `entryDate`, `closeoutDate`, `updateDate`) → Date  
    - Text fields (`stateName`, `declarationType`, `incidentType`, `disasterName`, `designatedIncidentTypes`) → Text  
    - Boolean flags (`iaProgramDeclared`, `ihProgramDeclared`, `paProgramDeclared`, `hmProgramDeclared`) → True/False  

 *Correct data types prevent calculation errors and ensure accurate aggregations.*

### 2.4 Handling Missing Values
- **To Do**: Identify and treat null values.  
- **Procedure**:
  - Use **Transform → Replace Values** for categorical fields.  
  - Apply conditional logic for dates:  
    - If `stateName` is missing → mark as `"Unknown"`.  
  - For `closeoutDate`:  
    - Null values indicate ongoing disasters.  
    - Retain nulls but add a **conditional column**:  
      - If `closeoutDate` is null → `"Open"`  
      - Else → `"Closed"`  

*Logical replacements ensure completeness without losing meaning.*


### 2.5 Creating Derived Columns
Derived fields enrich analysis beyond raw data.

- **Fiscal Year (`fyDeclared`)**:  
  - Formula: `Date.Year([declarationDate])` adjusted for fiscal cutoff (Oct–Sep).  
  - Example: Declaration on Nov 2020 → FY2021.  

- **Incident Duration**:  
  - Formula: `Duration.Days([incidentEndDate] - [incidentBeginDate])`.  
  - Example: Incident from Jan 1 to Jan 10 → 9 days.  

- **Status**:  
  - Formula: `if [closeoutDate] = null then "Open" else "Closed"`.  

*Derived columns allow trend analysis such as disasters per fiscal year, average duration, and open vs closed cases.*

### 2.6 Removing Duplicates
- **To Do**: Eliminate duplicate rows.  
- **Procedure**:
  - Go to **Home → Remove Rows → Remove Duplicates**.  

*Removing duplicates prevents double counting in dashboards.*


### 2.7 Loading Cleaned Data
- **To Do**: Save and apply transformations.  
- **Procedure**:
  - Click **Close & Apply** in Power Query.  
  - Load cleaned dataset into Power BI model.  

*The dataset is now ready for visualization.*

## 3. Final Outcome
By the end of the cleaning process:
- The FEMA dataset is **cleaned, standardized, and loaded** into Power BI.  
- Key derived fields (Fiscal Year, Incident Duration, Assistance Flags, Status) are done.  
- The dataset is **reliable for dashboards**, supporting accurate insights.  
