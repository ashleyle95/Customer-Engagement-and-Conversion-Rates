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
  - Flowchart:
    
 ![image](https://github.com/user-attachments/assets/cfb488fe-536e-44b3-999a-a60fc23ed7a0)
 
  - Data Transformation

 In this project, we will analyze and profile data within Power BI to assess its quality, completeness, and distribution. The goal is to ensure that the dataset is reliable for further analysis and reporting:  Data Overview, Data Quality Checks,  Descriptive Statistics & Distribution 
 our data profiling in Power BI revealed that most of the imported tables contain clean data. However, we made a few necessary adjustments:
 
✅ Removed 7 duplicate rows in the customer_journey table.

✅ Separated the ClickView Combined column in the engagement_data table using delimiters for better analysis.

 ## 3. Reporting Dashboard
[Embedded Demo in Power BI service](https://app.powerbi.com/view?r=eyJrIjoiMDA1MDRlZmYtNTgzYy00ZmYyLTllY2EtZmI4YjhjMWYxYjhjIiwidCI6IjA2N2UxZTE5LWExMWEtNDhlNS04Yjc5LTBiOWVlNzQ1YTdhMiJ9 )

The dashboard consists of four key pages, each providing in-depth insights into different aspects of marketing performance:

`Overview`: A high-level summary of key marketing metrics, including conversion rate, customer sentiment from reviews, and customer engagement on social media. This page highlights overall trends and areas requiring attention.

`Conversion Rate`: A detailed breakdown of conversion rates by product and day of the week, along with an analysis of the customer journey. This section helps identify patterns, bottlenecks, and opportunities for improving conversions.

`Customer Review Insights`: Incorporating sentiment analysis to evaluate customer feedback, this page helps understand customer experience, detect common concerns, and identify areas for product or service improvements.

`Social Media`: Analyzing customer interactions on social media to uncover engagement trends. This section provides insights into the effectiveness of marketing campaigns and helps refine strategies for better audience engagement.

## 4. Findings/Recommendations
()
## 5. Limitations
**In Python**

When analyzing sentiment, combining both the sentiment score and rating provides a more comprehensive understanding of the customer experience. By considering the sentiment expressed in the text along with the numerical rating provided by the customer, we can gain a more nuanced view of their overall satisfaction. However, there are some limitations when using both pre-trained models in data analysis:

Contextual Understanding: VADER relies on a predefined lexicon, which may fail to capture contextual nuances such as sarcasm or irony, leading to misinterpretations.

Polarity Misclassification: In some cases, BART might misinterpret the polarity (positive/negative/neutral) of a sentence if it’s subtle or mixed.

**In Power BI**

The sentiment categories include Strong Negative, Mixed Negative, Possibly Misclassified, Neutral, Strong Positive, and Mixed Positive. These classifications serve as assumptions for analysis and should be continuously monitored and validated to ensure long-term accuracy.

Based on sentiment analysis, we have categorized review topics into four main areas: Product Price, Product Quality, Delivery, and Customer Service. However, due to the complexity of customer reviews and potential misclassification, inaccuracies may arise, which could impact the reliability of data analysis.

To improve the accuracy of insights, it is recommended to avoid relying solely on sentiment analysis without considering external factors. Instead, integrating additional surveys and external data sources can enhance the depth and precision of the analysis, leading to more actionable recommendations.





