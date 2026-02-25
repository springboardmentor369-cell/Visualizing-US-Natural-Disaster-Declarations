# **Week 2: Power Query Data Cleaning Using On Customer Call Data**

This document outlines data cleaning and techniques in Power Query, specifically applied to a Customer Call Dataset. Building on the basic transformations from Week 1, this session focuses on methods essential for ensuring data quality in Power BI.

# **Data Cleaning Steps in Power BI (Power Query)**

This dataset contains customer information such as names, phone numbers, addresses, and flags like *Paying Customer* and *Do Not Contact*. Before analysis, the data must be cleaned to ensure accuracy, consistency, and usability.

---

## **Step 1: Load Data into Power BI**

1. Open **Power BI Desktop**  
2. Click **Home → Get Data**  
3. Select the source (Excel / CSV)  
4. Click **Transform Data** to open **Power Query Editor**

---

## **Step 2: Remove Unnecessary Columns**

* Identify columns that are not useful for analysis  
   Example: **Not\_Useful\_Column**  
* Select the column  
* Right-click → **Remove**

---

## **Step 3: Standardize Column Names**

* Rename columns for consistency and readability  
   Example:  
  * `First_Name` → `First Name`  
  * `Last_Name` → `Last Name`  
  * `Do_Not_Contact` → `Do Not Contact`  
* Right-click column header → **Rename**

---

## **Step 4: Handle Missing and Invalid Values**

### **Phone Number Column**

* Values like `N/a` or blank should be treated as missing  
* Select **Phone\_Number**  
* Click **Replace Values**  
  * Replace `N/a` with **null**  
* Change data type to **Text**

---

### **Address Column**

* Replace `N/a` with **null**  
* Trim extra spaces  
   **Transform → Format → Trim**

---

## **Step 5: Standardize Categorical Values**

### **Paying Customer Column**

The column contains mixed values like:

* `Yes`, `Y`, `No`, `N`, `N/a`

Steps:

1. Select **Paying Customer**  
2. Use **Replace Values**  
   * Replace `Y` → `Yes`  
   * Replace `N` → `No`  
   * Replace `N/a` → `null`

---

### **Do Not Contact Column**

* Standardize values:  
  * `Y` → `Yes`  
  * `N` → `No`  
* Replace blanks with `No` (if business rule allows)

---

## **Step 6: Fix Data Type Issues**

* `CustomerID` → **Whole Number**  
* Name columns → **Text**  
* Boolean columns (Yes/No) → **Text**  
* Verify each column using **Data Type icon**

---

## **Step 7: Remove Duplicate Records**

* CustomerID **1020** appears twice  
* Select **CustomerID**  
* Click **Remove Rows → Remove Duplicates**.

---

## **Step 8: Clean Name Fields**

* Remove unwanted characters  
   Example: `/White`, `...Potter`  
* Use **Replace Values** or **Transform → Format → Clean**

---

## **Step 9: Create Conditional Filtering Logic (Optional)**

* Exclude customers where:  
  * `Do Not Contact = Yes`  
  * or `Phone Number = null`

---

## **Step 10: Close and Apply**

* Click **Close & Apply**  
* Power BI loads the cleaned data into the model

