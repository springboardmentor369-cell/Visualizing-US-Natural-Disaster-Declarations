# Week 4: Importing Live Data into Power BI
Week 4 focused on understanding live data in Power BI and how real-time or continuously updating data can be imported, managed, and visualized. This week was particularly important as it helped me understand how data functions in real business environments, where information changes frequently and dashboards are expected to update automatically without manual effort.
 - Along with live data concepts, we were also introduced to GitHub as a professional platform to showcase our proof of work.
 - Understanding Live Data and Its Importance.
At the beginning of the week, we learned the concept of live data. Live data refers to data that updates in real time or at regular intervals, unlike static datasets that remain unchanged unless manually refreshed.

## Live data is critical in real-world applications such as:
* Sales and revenue tracking
* Customer support and ticketing systems
* Banking and financial transactions
* Operational monitoring dashboards
This helped me understand that manual updates are impractical in dynamic environments, making automation a necessity.

## Introduction to APIs and Their Role in Power BI
We were introduced to APIs (Application Programming Interfaces) and learned that APIs act as bridges that allow different systems to communicate and exchange data.
In Power BI, APIs play a key role by enabling:
* Direct connection to live data sources
* Automated data updates
* Real-time dashboard refreshes
*This clarified how modern dashboards stay updated without repeated manual data imports.
## Methods to Import Live Data into Power BI:
 - We explored different ways of importing live data, starting with Web data sources using URLs.
 - While attempting to import data from the NSE website, I learned an important limitation, All websites allow don't give direct data access. Due to security, privacy, and ethical restrictions, many platforms require proper authorization, API keys, or organization credentials.
 - This experience helped me understand why accessing real-time data is not always straightforward and must follow compliance rules.

## Understanding Data Refresh and Power BI Version Limitations:
* Another key learning was understanding how Power BI licensing impacts data refresh capabilities:
* Power BI Free: No automatic data refresh
* Power BI Pro: Allows up to 8 scheduled refreshes per day
This made it clear that tool limitations and licensing decisions directly affect how live data solutions are implemented.

## Live Data in the Context of Disaster Datasets
Since our project focused on disaster-related datasets, we discussed that live data may not always be necessary, as disasters do not occur continuously.
However, live data is extremely valuable in systems such as:
* Customer support platforms
* CRM and sales systems
* Financial and transaction-based platforms

- To better understand real-time data usage, we were introduced to the Zendesk platform, which demonstrated how live data functions in customer ticketing and support systems.
- Synthetic Data and Dummy Data
- We also learned the difference between dummy data and synthetic data:
- Dummy data: Simple sample data used for basic testing
- Synthetic data: Artificially generated data that closely resembles real-world data patterns
This concept was important because when real APIs are unavailable, synthetic data allows safe and ethical practice without violating security or privacy policies.

## Understanding ETL Pipelines
Another important concept introduced was ETL pipelines, which stand for:
* Extract – Collecting data from source systems
* Transform – Cleaning and structuring the data
* Load – Loading the data into Power BI
- ETL pipelines automate the entire data workflow and ensure that dashboards update automatically whenever the underlying data changes.

## Importance of Proof of Work and Introduction to GitHub
Proof of work : For this purpose, we were introduced to GitHub as a platform to showcase projects in a structured and transparent way.
GitHub Repository Structure Learned, We were guided to create a well-organized GitHub repository with the following structure:

## Structure of GitHub Repository 
### Data
Contains raw and processed datasets
### Power BI
Contains Power BI files and dashboards
### Data Cleaning
Contains screenshots and files documenting the data cleaning process
### Screenshots
Contains labeled screenshots showing the project workflow
### Documentation
Contains week-wise learning files  
### README File
We learned that the README file is especially important, as it provides an overview of the project and creates the first impression for viewers.

## Key Learnings from Week 4
* Live data enables automated and real-time dashboards
* APIs are essential for fetching continuously updating data
* Not all data sources are accessible due to security and privacy constraints
* ETL pipelines automate end-to-end data workflows
* GitHub is crucial for showcasing proof of work professionally
