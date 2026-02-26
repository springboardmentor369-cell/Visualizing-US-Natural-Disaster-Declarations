<<<<<<< HEAD
🌪️ Visualizing U.S. Natural Disaster Declarations 🇺🇸
📌 Project Overview

This project focuses on analyzing U.S. natural disaster declaration data to uncover patterns, trends, and regional impacts of disasters over time. Using interactive and static visualizations, the project helps transform complex FEMA data into meaningful insights 📈🗺️.

The analysis highlights:
📅 How disaster declarations change over time
🏛️ Which states are most affected
🌊 Which disaster types occur most frequently
📍 How disaster patterns vary by geography and incident type

❓ Problem Statement

The United States experiences a wide variety of natural disasters every year 🌪️🔥🌊. However, raw FEMA disaster data is large, complex, and difficult to interpret without proper analysis and visualization.

🎯 Objective
To analyze and visualize FEMA’s Disaster Declarations dataset in order to understand:
Trends in disaster declarations over the years
State-wise and regional disaster impact
Frequency of different disaster types
Geographic variation in disaster patterns

📂 Dataset Summary

Source: FEMA Disaster Declarations Dataset
Coverage: United States

📊 The dataset enables long-term trend analysis and regional comparison of disaster occurrences.

## 📁 Project Structure
```
Visualizing-US-Disaster-Declarations/
│
├── Data/
│   ├── raw/                          # Original FEMA datasets
│   ├── processed/                    # Cleaned and transformed data
│   └── external/                     # API imports and supplementary data
│
├── Data Cleaning/
│   ├── notebooks/                    # Jupyter notebooks for cleaning
│   ├── scripts/                      # Python cleaning pipeline
│   ├── power_query/                  # Power BI M transformations
│   └── logs/                         # Data quality logs
│
├── Documentation/
│   ├── Week1_Foundation.md
│   ├── Week2_Data_Quality.md
│   ├── Week3_EDA.md
│   ├── Week4_APIs_Git.md
│   ├── Week5_Visualization.md
│   ├── Week6_DAX.md
│   └── Final_Report.pdf
│
├── Power BI/
│   ├── dashboards/                   # .pbix files
│   ├── templates/                    # Reusable templates
│   ├── dax_library/                  # DAX measures library
│   └── documentation/                # User guides
│
├── Visuals/
│   ├── dashboards/                   # Dashboard screenshots
│   ├── individual_charts/            # Chart exports
│   ├── kpi_cards/                    # KPI visuals
│   └── presentations/                # Presentation-ready images
│
├── scripts/
│   ├── data_import.py                # API data fetching
│   ├── data_cleaning.py              # Cleaning pipeline
│   ├── eda_analysis.py               # Exploratory analysis
│   └── utils.py                      # Helper functions
│
├── notebooks/
│   ├── 01_Data_Profiling.ipynb
│   ├── 02_EDA.ipynb
│   └── 03_Statistical_Analysis.ipynb
│
├── requirements.txt                  # Python dependencies
├── .gitignore
├── LICENSE
└── README.md                         # This file
```

---


📊 KPI Usages

The following key performance indicators (KPIs) are used in the analysis:
🔢 Total number of disaster declarations
🗺️ Number of disasters by state
📅 Year-wise disaster trends
🌪️ Most common disaster types
📍 Regional distribution of disasters

🖥️ Dashboard Pages

The visual analysis is organized into multiple views:

📅 Time-Based Analysis
Disaster declarations by year
Trend analysis over decades

🗺️ State & Regional Analysis
Most affected states
Region-wise disaster comparison

🌊 Disaster Type Analysis
Frequency of disaster types (Flood, Hurricane, Fire, etc.)
Comparison of incident types across regions

🔍 Key Insights

📈 Disaster declarations have increased over time, especially after the 2000s
🏛️ Certain states experience disasters far more frequently than others
🌊 Floods, hurricanes, and severe storms are among the most common disaster types
📍 Coastal and southern regions show higher disaster concentration

✅ Recommendations

🛡️ States with high disaster frequency should strengthen disaster preparedness and response planning
📊 Historical trends should be used to improve risk assessment and resource allocation
🌍 Region-specific disaster mitigation strategies can reduce long-term impacts
🔄 Continuous monitoring of disaster data can help policymakers make data-driven decisions

🛠️ Tools & Technologies Used

🐍 Python – Core programming language

🐼 Pandas – Data loading, cleaning, transformation, and aggregation

🔢 NumPy – Numerical computations

📉 Matplotlib – Customized data visualizations

🎨 Seaborn – Statistical and exploratory visualizations

📊 Power BI – Interactive dashboards, KPI tracking, and visual storytelling

📓 Jupyter Notebook / JupyterLab – Interactive analysis and documentation

🚀 Conclusion

This project demonstrates how data analysis and visualization can simplify complex disaster datasets and reveal actionable insights. By understanding disaster trends and geographic impact, stakeholders can make better-informed decisions for disaster preparedness and risk management 🌍📊.
=======
Visualizing US Natural Disaster Declarations (FEMA Data)

📌 Project Overview

This project analyzes and visualizes natural disaster declarations in the United States using FEMA data. Interactive dashboards and KPIs help stakeholders understand disaster patterns, frequency, and impact, enabling better emergency preparedness and decision-making.

⚠️ Problem Statement

Natural disasters significantly affect communities and economies in the U.S., but tracking patterns and trends across states and disaster types is challenging due to the complexity of FEMA data. This project addresses the need for:

Quick visualization of disaster trends

Identifying most affected states and disaster types

Tracking tribal assistance requests and disaster impact

📊 Dataset Description

The FEMA dataset contains historical and recent disaster declarations with key fields:

Column	Description
Disaster Number	Unique ID for each disaster declaration
Incident Type	Type of disaster (Flood, Hurricane, Tornado, etc.)
State	U.S. state where the disaster occurred
Declaration Date	Date when the disaster was declared
Incident Begin/End Date	Duration of the disaster
Cost & Impact	Estimated damage cost, people affected
Assistance Requests	Requests for federal aid, including tribal communities

Source: FEMA Open Data

📈 Key Performance Indicators (KPIs)

Total Disasters by Year – Annual count of declarations

Disasters by Type – Most frequent disaster types

People Affected – Impact per disaster type/year

Cost of Disasters – Financial impact per disaster type/year

State-wise Disaster Frequency – Most disaster-prone states

Tribal Assistance Requests – Count and type per disaster

🔍 Key Insights

California, Texas, and Florida have the highest disaster frequency.

Floods and hurricanes are the most common; tornadoes and wildfires have high localized impact.

Hurricanes cause the highest financial damage.

Tribal assistance requests highlight the need for tailored emergency planning.

💡 Recommendations (Future Improvements)

Integrate real-time FEMA data for live dashboards.

Predict disasters using machine learning based on historical trends.

Include geographic maps for county- and state-level analysis.

Combine socio-economic data to assess disaster vulnerability and aid allocation efficiency.

🛠 Tools Used

Power BI – Interactive dashboards and KPI visualization

Python (Pandas, NumPy) – Data cleaning and transformation

Excel / CSV – Dataset management

DAX – Custom calculations for KPIs

📌 Project Status

Task	Status

Data Collection & Cleaning	✅ Completed

Dashboard & KPIs	✅ Completed

Insights Analysis	✅ Completed

Predictive Modeling	⚠️ Planned

Real-Time Data Integration	⚠️ Planned

📸 Screenshots

Dashboard Overview:


Disasters by Type:


State-wise Impact:


👤 Author

Sanaka Mounika

Data Analyst | Power BI Developer

Email: mounasanaka@gmail.com
>>>>>>> 907efb0a3d3ca6feb32f0512c7808b36508efac5
