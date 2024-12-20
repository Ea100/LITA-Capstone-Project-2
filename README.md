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

### Data Analysis
---
```SQL
SELECT top 5 subscriptionType,COUNT(CustomerID) AS TOTAL_CUSTOMER
from[dbo].[LITA Customer Data]
GROUP BY SubscriptionType
```

### Data Visualizations
---
![SQL CustomerData 1](https://github.com/user-attachments/assets/ccb48c42-60e3-47cc-a6d9-0fc746b48d20)
![SQL CustomerData 2](https://github.com/user-attachments/assets/33660d25-19ea-48b6-ba90-d3bd8c51aa5c)
![Subscription Performance Dashboard (Excel)](https://github.com/user-attachments/assets/8af7d036-87a2-4bea-abed-669f008a8664)
![CustomerData BI Dashboard](https://github.com/user-attachments/assets/789ce9de-e9d4-420b-8b6a-75f26e681da5)


### Results/Findings
---
The analysis results are summarized as follows:
- The Basic subscription is the most popular, with 37,500 customers, followed by Premium and Standard, each with 18,750 customers
- Basic subscriptions generate the highest revenue at approximately $74.8 million, followed by Premium with $37.6 million, and Standard with $37.5 million.
- For the "Churn Rate Analysis by Region", the East and South regions have the highest number of cancellations, with 11,250 each while the North and West regions have the lowest number of cancellations, with 7,500 each.
- Based on the "Cancellations by Subscription Type":
  1. Basic: Out of 37,500 customers, 11,250 canceled (approximately 30% churn rate).
  2. Premium: Out of 18,750 customers, 11,250 canceled (approximately 60% churn rate).
  3. Standard: Out of 18,750 customers, 11,250 canceled (also approximately 60% churn rate).

### Limitations
---
- The data does not provide insights into specific customer preferences or reasons for cancellations
