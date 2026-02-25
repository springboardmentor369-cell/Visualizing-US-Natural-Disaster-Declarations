# 📊 **Visualizing US Natural Disaster Declarations**
**(FEMA Dataset – End-to-End Data Analytics Project)**

---

## 🔍 **Project Overview**

Natural disasters pose persistent risks to **human life, infrastructure, and public resources** across the United States. While FEMA provides comprehensive disaster declaration data, extracting meaningful insights from decades of raw records is challenging without structured analytics and visualization.

This project presents an **end-to-end data analytics solution** that transforms FEMA disaster declaration data into **decision-support dashboards**. Using **systematic data cleaning**, **business-focused exploratory data analysis**, and **interactive Power BI visualizations**, the project enables stakeholders to understand:

- **Where disaster risk is concentrated**
- **How disaster risk evolves over time**
- **Which regions and disaster types should be prioritized**

The focus of this project is **not just visualization**, but **answering real-world analytical questions** aligned with professional decision-making scenarios.

---

## 🎯 **Problem Statement**

Instead of building generic dashboards, this project is structured around **two high-impact analytical questions**, each addressed using a dedicated dashboard.

### **Core Questions**

1. **Which states should be prioritized for disaster preparedness and mitigation?**
2. **How has national disaster risk evolved over time, and what does this imply for future preparedness?**

These questions are critical for:
- **Government agencies**
- **Disaster management authorities**
- **Emergency planners**
- **Policy and funding decision-makers**

---

## 📁 **Dataset Description**

- **Source:** FEMA Disaster Declarations Dataset  
- **Geographic Scope:** United States (States & Territories)  
- **Time Period:** 1953 – 2025  

### **Key Attributes**
- **Disaster declaration dates**
- **State and geographic location**
- **Disaster / incident type (Flood, Storm, Tornado, etc.)**
- **Declaration frequency and outcomes**

This dataset represents **real-world operational data**, making it suitable for **applied analytics and decision support**.

---

## 🧹 **Data Cleaning & Preparation**

Before visualization, the dataset underwent **structured preparation** to ensure analytical accuracy:

- **Verified missing values** across all columns  
- **Retained missing incident end dates**, as many disasters are single-day or ongoing events  
- **Removed non-analytical identifier columns**  
- **Standardized data types**:
  - **Dates → Date format**
  - **Numerical fields → Numeric**
  - **Categorical attributes → Text**

After cleaning, the refined dataset was imported into **Power BI** for modeling and visualization.

---

## 📊 **Exploratory Data Analysis (Business-Focused)**

Exploratory Data Analysis (EDA) was performed with a **business and policy lens**, focusing on:

- **Year-wise variation in disaster declarations**
- **Identification of consistently high-impact states**
- **Dominant disaster types across decades**
- **Detection of abnormal spikes and long-term trends**

Insights from EDA directly guided:
- **KPI selection**
- **Chart types**
- **Dashboard structure**

This ensured that **every visual answers a specific analytical question**, rather than displaying raw counts.

---

## 📌 **KPIs & Measures Designed**

To support **high-level decision-making**, the following KPIs were created using DAX:

- **Total Disaster Declarations**
- **High-Risk States Count** (states above national average)
- **Top Impact State**
- **Most Frequent Disaster Type**
- **Peak Year & Peak Year Declarations**
- **Average Annual Declarations**

These KPIs provide **instant context on scale, severity, and prioritization**.

---

## 📈 **Dashboard Design & Question-Driven Analysis**

### **Dashboard 1 — Regional Disaster Risk & Funding Priority**

#### **Business Question Addressed**
**Which states should be prioritized for disaster preparedness and mitigation?**

#### **Why This Question Matters**
Disaster preparedness resources are **limited**, and identifying where risk is concentrated ensures **maximum impact of funding and mitigation efforts**.

#### **Key Visuals Used**
- **KPI Cards**
  - **Total Declarations**
  - **Top Disaster Type**
  - **Top Impact State**
- **Top States by Disaster Declarations (Bar Chart)**
- **Geographic Map (State-wise Distribution)**

#### **How the Dashboard Solves the Question**
- States exceeding the **national average** are classified as **high-risk**
- Ranking enables **clear funding prioritization**
- Disaster type insights support **targeted mitigation strategies**

#### **Outcome**
This dashboard provides a **clear, actionable view of regional disaster risk**, enabling stakeholders to **prioritize states and disaster types** for preparedness and resource allocation.

---

### **Dashboard 2 — Disaster Trend & National Risk Analysis**

#### **Business Question Addressed**
**How has disaster risk evolved over time, and what does this imply for future preparedness?**

#### **Why This Question Matters**
Understanding historical trends helps distinguish between:
- **Short-term fluctuations**
- **Long-term structural risk growth**
- **Extreme peak scenarios**

This is essential for **strategic, long-term planning**.

#### **Key Visuals Used**
- **Annual Disaster Declarations Trend (1953–2025)**
- **Peak Year Highlight**
- **Decade-wise Aggregation**
- **Executive KPIs**
  - **Peak Year**
  - **Peak Year Declarations**
  - **Average Annual Declarations**

#### **How the Dashboard Solves the Question**
- Reveals a **long-term upward trend** in disaster declarations
- Highlights **extreme historical years** requiring contingency planning
- Enables comparison of **risk patterns across decades**

#### **Outcome**
This dashboard supports **national-level disaster risk assessment**, helping policymakers plan for both **average conditions and worst-case scenarios**.

---

## 💡 **Key Insights**

- Disaster declarations show a **long-term increasing trend**, with notable historical spikes
- **Floods and severe storms** dominate disaster frequency nationwide
- **A limited number of states** contribute disproportionately to total disaster declarations
- Disaster risk varies significantly **across decades**, indicating evolving exposure and reporting patterns

---

## 📌 **Recommendations**

- **Prioritize preparedness and mitigation efforts** in high-risk states
- **Focus infrastructure investments** on dominant disaster types such as floods
- **Leverage historical trends** for future predictive modeling
- **Shift from reactive response to proactive disaster planning**

---

## 🛠 **Tools & Technologies Used**

- **Python** – Data cleaning and preprocessing
- **Pandas & NumPy** – Data transformation
- **Power BI Desktop** – Data modeling, DAX measures, interactive dashboards
- **Jupyter Notebook** – EDA and documentation
- **GitHub** – Version control and project sharing

---

## **Images**

<img width="1429" height="796" alt="Screenshot 2026-02-19 101551" src="https://github.com/user-attachments/assets/8f161933-16d6-4687-9448-5ba79e12aec3" />
<img width="1445" height="808" alt="Screenshot 2026-02-19 101606" src="https://github.com/user-attachments/assets/4df17e59-5158-44f8-8d54-96a988956ca1" />

---

## 🏁 **Project Outcome**

This project demonstrates a **complete data analytics lifecycle** — from raw data preparation and **business-driven exploratory analysis** to **question-focused dashboards** that support **real-world decision-making** in disaster management and policy planning.
