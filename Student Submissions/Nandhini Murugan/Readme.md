# 🌪️ **Visualizing US Natural Disaster Declaration**

# 📌 **Problem Statement**

The frequency and intensity of natural disasters in the United States pose significant challenges to emergency management and resource distribution. This project visualizes historical disaster declaration data to identify geographic hotspots, temporal trends, and high-impact incident types to support better disaster preparedness and mitigation strategies.

# 📊 **Dataset Description**

The dataset consists of 68,542 records detailing federal disaster declarations in the US from 1953 to 2024 consisting total column of 24.

📂 Dataset Name:
DisasterDeclarationsSummaries - Cleaned Dataset

The dataset contains federal disaster declaration records across U.S. states, including:

🔑 Key Columns Used

- declarationType – Type of declaration (DR, EM, FM)

- incidentType – Disaster category (Severe Storm, Flood, Hurricane, etc.)

- state – Affected state

- declarationDate – Date federal declaration was issued

- fyDeclared – Fiscal year of declaration

- designatedArea – County-level affected areas

- disasterNumber – Unique disaster identifier

📌 The dataset enables descriptive and strategic disaster analysis.

# 📈 **Key Performance Indicators (KPIs)**

The KPIs were designed to move beyond reporting and support strategic decision-making.

📈Impact & Trend KPIs and Risk Analysis

- 1.Total Disaster Declarations

  - Measures overall disaster exposure scale.

- 2.Total States Affected

  - Indicates geographic spread of disasters.

- 3.Total Incident Types

  - Shows hazard diversity.

- 4.Most Frequent Disaster Type

  - Identifies dominant hazard category.

- 5.Latest Year Total Declarations

  - Monitors recent disaster activity.

# 📊 **Dashboard Pages**

## 📍Page 1: US Natural Disaster Impact & Trend Analysis

🎯 Purpose:
To provide descriptive insights into disaster frequency, geographic distribution, and hazard composition.

📊 Visuals Used:

- 🧮 KPI Cards

- 📈 Trend line chart (Declarations by Year)

- 📊 Stacked bar (Incident Type by Year)

- 📊 Bar chart (Incident Type by Declaration Type)

- 🗺️ Map (State-level distribution)

- 🎛️ Slicers (Incident Type, Year Declared)

❓ This page answers:

- What is happening?

- Where are disasters concentrated?

- Which types dominate?

- How have trends changed over time?


# 🔎 **Key Insights**

1. 🌩️ Severe Storm is the most frequent disaster type across years.

2. 📍 Certain states (e.g., Texas) show consistently high vulnerability.

3. 📊 Disaster trends peaked around 2020 and show long-term fluctuation.

# 💡 **Recommendations**

**🔹 Add More Recent Data**

Regularly update the dataset to keep the dashboard accurate and aligned with current disaster trends.

**🔹 Add More KPIs**

Include additional metrics like average disasters per year, most affected state, or yearly growth percentage for deeper insights.

**🔹 Improve Dashboard Design & Formatting**

Enhance visual consistency using better color themes, alignment, and clear labels to make the dashboard more professional and easy to understand.

# 🛠️ **Tools Used**

**📊 Power BI:** Used for data cleaning, modeling, and dashboard development. Power Query helped transform and prepare the dataset for analysis. DAX was used to create key measures. It enabled the creation of interactive visuals, maps, and slicers to analyze disaster trends and preparedness insights.

**🐍 Google Colab:** Used as the primary environment for data cleaning. Python (Pandas) scripts were executed in Colab to handle missing values, clean strings, and format the dates before exporting the final CSV for visualization.

**💻 VS Code:** The primary Integrated Development Environment (IDE) used to write and run the Jupyter Notebooks and manage project documentation.

**🔄 Git:** Employed for version control to track changes in the data cleaning scripts and the README file.

**🌐 GitHub:** Used to store, manage, and share the project repository, ensuring the analysis is accessible and reproducible.

### 👩‍💻 **Author** - Nandhini Murugan
🎓 Internship at Infosys Springboard
