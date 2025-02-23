![image](https://github.com/user-attachments/assets/b1a3fe7d-025a-4b3b-ade0-81eedcde2a83)
# PROJECT: Customer Engagement and Conversion Rates
## Project Links
[Python-Sentiment Analysis - Customer Review](https://github.com/ashleyle95/Customer-Engagement-and-Conversion-Rates/blob/main/Sentiment%20Analysis-Customer%20Review%20(4).ipynb)

[PowerBI-Interactive Dashboard](https://app.powerbi.com/view?r=eyJrIjoiMDA1MDRlZmYtNTgzYy00ZmYyLTllY2EtZmI4YjhjMWYxYjhjIiwidCI6IjA2N2UxZTE5LWExMWEtNDhlNS04Yjc5LTBiOWVlNzQ1YTdhMiJ9)

[Measures - Power BI (Notion Link)]

[Final Report-Presentation]()

## Table of contents
[1. Project Overview](#1-project-overview)

[2. Data Process](#2-data-process) 

[3. Reporting Dashboard](#3-reporting-dashboard)

[4. Findings/Recommendations](#4-findingsrecommendations)

[5. Limitations](#5-limitations)

## 1. Project Overview

### Context

An online retail business, A, is addressing the decline in customer engagement and conversion rates due to the underperformance of marketing campaigns, which did not yield the expected return on investment.
 A more detailed analysis is required to identify areas for improvement in the marketing strategies, as higher marketing expenditures are not translating into the anticipated returns. Additionally, the analysis should focus on understanding customer feedback to inform strategies that can enhance customer engagement and increase conversion rates.

Highlight KPI:

+ Conversion rate: % web visitors who make a purchase
+ Customer Engagement Rate: Level of interactions with marketing content (clicks, comments, likes)
+ Average Order Value (AOV): average amount spent by a customer  per transaction
+ Customer Feedback Score: Average rating from customer reviews

### Objective

+ Increase Conversion Rates:
Goal: Identify factors impacting the conversion rate and provide recommendations to improve it.
Insight: Highlight key stages where visitors drop off and suggest improvements to optimize the conversion funnel.

+ Enhance Customer Engagement:
Goal: Determine which types of content drive the highest engagement. 
Insight: Analyze interaction levels with different types of marketing content to inform better content strategies.

+ Improve Customer Feedback Scores:
Goal: Understand common themes in customer reviews and provide actionable insights.
Insight: Identify recurring positive and negative feedback to guide product and service improvements.

### Data sources

Restore database `File PortfolioProject_MarketingAnalytics.bak` in SQL Server that includes tables as below:

+ `dim_customers`: details of customers
  ![image](https://github.com/user-attachments/assets/9736fd6a-6603-4c53-8f9d-d2ca8708a870)
+ `dim_geography`: name of countries and cities
  ![image](https://github.com/user-attachments/assets/fff80ee9-2b12-48ac-9f72-0e36db30f348)
+ `dim_products`: details of products
  ![image](https://github.com/user-attachments/assets/a39cbe26-e618-4586-8cb3-f9156cfbc44c)
+ `customer_journey`: records of customer journey in the webstite through actions: views, clicks, dropoff, purchase
  ![image](https://github.com/user-attachments/assets/848d62ee-2380-4a72-b82e-00f397f97a67)
+ `customer_reviews`: records of customer reviews
  ![image](https://github.com/user-attachments/assets/ad6c21ca-219f-4a79-8cac-0fea740ffb12)
+ `engagement_data`: records of customer engagements on the marketing campaigns
  ![image](https://github.com/user-attachments/assets/0734c568-c4c9-4260-91c4-571532a88c38)

## 2. Data Process  
  - Data Processing:
     + SQL server to restore backup database file`.bak`
     + Python: Sentiment Analysis file `customer_reviews` 
  - Reporting/Visualisation: PowerBI
    



