# **Week 4: Real-Time Data and External Data Sources (APIs, CRM, Zendesk)**

This document summarizes the concepts covered in Week 4, focusing on the use of live data, its application in disaster datasets, and methods for connecting to various external data sources such as APIs, CRM systems, and Zendesk. Understanding these concepts is critical for building dynamic, up-to-date reporting and analysis.

# **Introduction to Live Data**

Live data, or real-time data, refers to data that is continuously generated and delivered immediately after it is collected. Unlike static, batch-processed data, live data allows for instant monitoring and rapid decision-making.

# **Connecting to External Data Sources**

In addition to traditional file or database sources, modern analysis often requires integrating data from specialized online platforms. This session covered how to connect to these sources using APIs.

## **1\. APIs (Application Programming Interfaces)**

An API acts as a middleman, allowing different software applications to communicate and share data securely.

| API Concept | Description |
| :---- | :---- |
| **What it is** | A set of rules that defines how one piece of software can interact with another. |
| **Why use it** | To get live or semi-live data directly from the source system (e.g., stock prices, weather updates). |
| **Method in Power BI** | Using the **Web** data connector and specifying the URL and required authentication. |

## **2\. CRM (Customer Relationship Management) Systems**

CRM systems store all information related to an organization's customers, including sales, marketing, and service data.

* **Examples:** Salesforce, HubSpot.  
* **Data typically accessed:** Customer profiles, sales pipelines, order history.  
* **Integration:** Often connected through native Power BI connectors or custom APIs.

## **3\. Zendesk**

Zendesk is a popular customer service and support platform that centralizes customer interactions, support tickets, and knowledge bases.

* **Purpose:** Analyzing customer service efficiency, ticket resolution times, and customer satisfaction scores.  
* **Key Data Points:** Ticket status, agent performance, customer feedback scores.  
* **Integration:** Power BI has a dedicated connector to pull data directly from the Zendesk API.

To access data from these sources in Power BI, one must typically perform the following actions:

1. Obtain necessary **API Keys** or **Security Tokens** for authentication.  
2. Use the **Get Data → Web** or a **Dedicated Connector** (e.g., Zendesk connector).  
3. Load the data into the Power Query Editor for initial transformation and cleaning.

