# Visualizing US Natural Disaster Declaration: Trends and Patterns

## Problem Statement:
Disasters in the United States — ranging from hurricanes and floods to wildfires and pandemics — trigger federal declarations that activate critical assistance programs. While FEMA provides extensive data on these declarations, the raw dataset is complex and difficult to interpret without specialized tools.
This project addresses the challenge by transforming FEMA’s Disaster Declarations dataset into interactive dashboards that:

- Summarize disaster activity across years, states, and incident types.

- Reveal temporal trends, durations, and seasonal patterns of disasters.

- Track activation of Individual Assistance (IA), Individual and Household Programs (IH), Hazard Mitigation Assistance (HMA) and Public Assistance (PA).

- Compare disaster types to assess severity and recurrence.

- Provide historical insights and predictive signals to support planning and resource allocation.

## Dataset Description:
- **Source:** FEMA Disaster Declarations dataset (OpenFEMA API / CSV download).

- **Size:** ~100,000+ records, 30+ columns.

- **Fields used:**

    - disasterNumber, stateName, incidentType, declarationType, declarationDate, closeoutDate.

- **Fields Created:**
    - FyDeclared, incidentDuration, status, requestingTime, programs. 

## KPIs Used:
- **Count of disasterNumber:**  Total number of disasters declared.

- **Average incidentDuration:**  Mean duration of disasters in days.

- **Average requestingTime:**  Mean time taken to process disaster requests.

- **Closed vs Open status ratio:**  Percentage of disasters resolved vs ongoing.

- **Program activation counts:**  IA, IH, HMA, PA activations across states.

- **Seasonality patterns:**  Average disasters per month.

## Dashboard Pages:
### 1. Disaster Overview and Trends
**Charts:**

- **Line chart:** Disasters declared per fiscal year.

- **Pie chart:** Distribution of declaration types (Major Disaster, Fire Management, Emergency, Fire Suppression).

- **Bar chart:** Frequency of each incident type (Fire, Flood, Hurricane, Tornado, etc.) and Frequency of disasters over Month.


*Question answered: What types of disasters are most frequently declared, and which states/regions experience the highest number of disasters?*

### 2. Process & Timelines
**Charts:**

- **KPI card:** Average requesting time vs target benchmark (< 5 days).

- **Line chart:** Requesting time trend by fiscal year.

- **Bar chart:** Requesting time by state.

- **Pie chart:** Disaster status (Closed vs Open).

- **Stacked bar chart:** Program activations by state.

*Question answered: How efficient is FEMA’s disaster response process — in terms of average request processing time, closure rates, and program activation timelines?*

## Key Insights:
***Disaster Overview:***

- Major Disasters dominate declarations (~60%).

- Fire, Severe storms, and Hurricanes are the most frequent incident types.

- States like Texas, Florida, and California consistently lead in disaster counts.

***Process & Timelines:***

- Average request processing time is ~33 days, far above the benchmark of 5 days.

- Closure rates are strong (73% closed), but ~27% remain open.

- Certain states (e.g., Marshall Islands, Micronesia) show extreme delays in processing.

- PA and IA programs are most frequently activated, reflecting large‑scale infrastructure and individual recovery needs.

## Recommendation:
  Enhance usability by adding customizable filters and role‑based views so different stakeholders see what matters most. Incorporate anomaly detection alerts that automatically flag unusual patterns in the data. Use progressive disclosure, showing high‑level KPIs first and allowing deeper drill‑downs only when needed. Finally, embed contextual notes or benchmarks alongside metrics to help users interpret numbers in real time.

## Tools Used:
- **POWER BI:** To clean, load and visualize the data
- **VS CODE:** To clean the dataset using *Python*
- **GITHUB:** To showcase this project

