# LITA-Capstone-Project-2
The project analyzed customer data from a subscription service to understand subscription patterns, customer segments, and retention trends. Excel was used for pivot table analysis, followed by SQL queries to identify popular subscription types, cancellation trends, and revenue by segment.

### Project Title: Customer Segmentation for a Subscription Service

[Project Overview](#project-overview)

[Data Sources](#data-sources)

[Tools Used](#tools-used)

[Exploratory Data Analysis](#exploratory-data-analysis)

[Data Analysis](#data-analysis)

### Project Overview
---
This project aimed to analyze customer data from a subscription service to understand subscription patterns, customer segments, and retention trends. Excel was initially used for pivot table analysis to examine subscription types, average durations, and regional distributions. SQL queries further identified customer behaviour insights, such as popular subscription types, cancellation trends, and revenue by segment. The final Power BI dashboard presents a comprehensive view of customer segments, highlighting opportunities to improve retention and optimize subscription offerings.

### Data Sources
---
Customer data for this project was also sourced from the "LITA Capstone Dataset.xlsx" file, which includes customer profiles, subscription types, revenue, and cancellation details. This data was converted to a CSV format for import into SQL Server to facilitate SQL-based analysis.

### Tools Used
---
- Microsoft Excel [Download Here](https://www.microsoft.com)
  1. For Data Cleaning
  2. For Analysis
  3. For Data Visualization
  - SQL – Structured Query Language for querying of Data
  - PowerBI - Used for creating an interactive dashboard to visualize key insights
  - GitHub for Portfolio Building

### Exploratory Data Analysis
---
EDA questions aimed to reveal customer behaviour, subscription popularity, and cancellation patterns:
- What are the most popular subscription types by customer count?
- What is the average subscription duration across all customers?
- How does the cancellation rate vary by subscription type?
- Which regions have the highest and lowest number of cancellations?
- What percentage of total revenue is contributed by each subscription type?

### Data Analysis
---
```SQL
SELECT top 5 subscriptionType,COUNT(CustomerID) AS TOTAL_CUSTOMER
from[dbo].[LITA Customer Data]
GROUP BY SubscriptionType
```

### Data Visualizations
![SQL CustomerData 1](https://github.com/user-attachments/assets/ccb48c42-60e3-47cc-a6d9-0fc746b48d20)
![SQL CustomerData 2](https://github.com/user-attachments/assets/33660d25-19ea-48b6-ba90-d3bd8c51aa5c)


### Results/Findings
The analysis results are summarized as follows

### Recommendations
Based on the analysis carried out, we recommend the following:

### Limitations


