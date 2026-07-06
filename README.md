# Customer-Churn-Analysis-Banking-Power-BI
An end-to-end Business Intelligence project analyzing customer churn in the banking industry using Power BI. The project covers Power Query ETL, dimensional data modeling, DAX development, AI-powered customer segmentation, interactive dashboards, and business-driven recommendations to identify churn drivers and support retention strategies.
<img width="1232" height="734" alt="image" src="https://github.com/user-attachments/assets/a2fb5ff1-9b8b-4bca-a310-27415ff344b9" />

# Project Overview #

## 1. Background & Business Problem
**Business Context**

Customer churn is a major challenge for retail banks, impacting revenue and long-term profitability. This project aims to analyze customer behavior, identify churn drivers, and uncover high-risk customer segments to support data-driven retention strategies.

**This dashboard aims to help management answer the following business questions:**

- What is the overall customer churn rate and how has it changed over time?
- Which customer segments have the highest risk of churn?
- What customer characteristics are most associated with churn?
- Which demographic and behavioral factors influence customer retention?
- What actions can the bank take to reduce churn and improve customer loyalty?

**The analysis focuses on:**

- Customer Churn: Churn Rate, Churn Balance, Retained Customers
- Customer Segmentation: Age, Gender, Geography, Tenure, Balance, Salary, Credit Score
- Customer Behavior: Active Membership, Credit Card Ownership, Product Usage
- High-Risk Segments: AI Key Influencers & Top Segment Analysis
- Business Goal: Customer Retention & Churn Reduction Strategy

## 2. Project Objective

- Analyze the overall customer churn rate and customer retention performance.
- Identify the key factors driving customer churn using customer demographics and behavioral attributes.
- Discover high-risk customer segments through AI-powered Key Influencers and segmentation analysis.
- Provide actionable business recommendations to improve customer retention and reduce churn.
- Build an interactive multi-page Power BI dashboard to support data-driven decision-making.

# Dataset Description & Data Structure #

The dataset contains customer demographic, financial, and behavioral information from a retail bank to analyze customer churn patterns and identify factors influencing customer retention.
- Data Volume: 10,000 Customers
  <img width="1186" height="572" alt="image" src="https://github.com/user-attachments/assets/0326f811-0e59-49fc-a3ae-f5fc6f32c8b5" />
- 1 Fact Table: Customer
- 8 Dimension Tables: Geography, Gender, Age Group, Balance Group, Credit Score Group, Salary Group, Active Member, Credit Card
- Data Model: Star Schema <img width="1720" height="960" alt="image" src="https://github.com/user-attachments/assets/20b65af9-53b6-42ea-bcf8-78d06603185b" />

# Design Thinking Process #
## Step 1. Empathize ##
- 5W1H <img width="1414" height="680" alt="image" src="https://github.com/user-attachments/assets/43ff38da-e37a-4582-92c8-9fb41441e81f" />
- Empathy Map <img width="1686" height="796" alt="image" src="https://github.com/user-attachments/assets/655b7f76-44a1-4f35-9d65-ac762632bcbe" />
**Key Questions**
- What is the current customer churn rate?
- Which customer segments have the highest churn risk?
- What factors contribute most to customer churn?
- How do customer demographics and behaviors affect churn?
- Which customers should be prioritized for retention?

## Step 2: Define Point of View ##
- North Star Metrics <img width="1414" height="620" alt="image" src="https://github.com/user-attachments/assets/8eaab713-5b26-46ef-850e-329d6ce74863" />
- Define Point of View <img width="1420" height="536" alt="image" src="https://github.com/user-attachments/assets/aad24dea-7b9c-4125-a806-298579946c21" />
- Business Metrics Framework <img width="1406" height="510" alt="image" src="https://github.com/user-attachments/assets/c51eb529-c84b-4430-9153-50f482b8d731" />

# Key Insights & Visualizations #

## Data Preparation & Modeling ##
Before building the dashboard, the dataset underwent exploratory data analysis (EDA), data cleaning, and business-oriented transformation to improve analytical quality and support dimensional modeling.

**Key Tasks**
- Performed Exploratory Data Analysis (EDA) to understand customer characteristics and identify churn patterns.
- Cleaned and validated the dataset by reviewing data types, missing values, and data consistency.
- Created business-oriented grouping dimensions, including Age Group, Balance Group, Salary Group, Credit Score Group, and Tenure Group, to support more meaningful customer segmentation.
- Designed a Star Schema by separating the customer fact table from multiple dimension tables.
- Developed DAX measures and dynamic parameter tables for interactive analysis.

## Customer Churn Overview ##
The Overview page provides a comprehensive view of customer churn performance across different demographic and behavioral dimensions. It helps identify major churn patterns, compare customer groups, and uncover the key factors associated with customer attrition before conducting a deeper segment analysis.
<img width="1788" height="1006" alt="image" src="https://github.com/user-attachments/assets/9c22320e-36a7-451d-9144-9d6c1c113f37" />

**Key Findings**
- Overall churn rate is 20.37%, with 2,037 out of 10,000 customers leaving the bank.
- 64% of churned customers are inactive members, suggesting customer disengagement is one of the strongest churn indicators.
- Germany records the highest churn rate (32.44%), nearly double that of France (16.15%) and Spain (16.67%).
- Female customers have a significantly higher churn rate (25.07%) than male customers (16.46%).
- Customers aged over 41 years consistently exhibit higher churn rates than younger age groups.
- Customers without a credit card show a 27% churn rate, compared with only 15% for customers who own a credit card.
- No significant differences in churn were observed across tenure, account balance, estimated salary, or credit score at the overall customer level.
- During January, the bank lost an average of 65.7 customers per day, with Monday, Tuesday, Wednesday, and Friday recording churn levels approximately 2–3% above the daily average.

**Business Interpretation**
The overview analysis indicates that customer engagement, geography, age, gender, and product adoption are the primary drivers of churn. These findings provide the foundation for a deeper investigation into the four AI-identified high-risk customer segments, where retention opportunities can be analyzed in greater detail.

## High-Risk Segment 1 – Female Customers Aged ≥51 ##
This dashboard investigates the highest-risk customer segment identified by the AI Key Influencers visual. The objective is to understand which business characteristics further increase churn risk within mature female customers.
<img width="1516" height="1000" alt="image" src="https://github.com/user-attachments/assets/bb348bb1-3834-42c8-98b4-7dfd8d79d4dd" />

**Key Findings**
- The segment contains 319 churned customers and 285 retained customers, resulting in a 52.8% churn rate, the highest among all identified segments.
- Germany records the highest churn rate at 67.03%, compared with 48.94% in France and 42.14% in Spain.
- Customers with medium account balances (€100k–150k) contribute the largest amount of churned balance (€16.08M) and exhibit a churn rate of 69.77%.
- Customers with poor credit scores (<580) consistently experience higher churn than those with fair or excellent credit scores.
- More than 62% of customers in this segment own a credit card, indicating that credit card ownership alone is insufficient to retain this high-risk group.

**Business Implications**
This segment represents the highest priority for retention initiatives, particularly mature female customers in Germany with medium account balances. Personalized financial advisory services and premium retention programs should be considered.

## High-Risk Segment 2 – Germany Customers Aged 41–50 ##
<img width="1462" height="952" alt="image" src="https://github.com/user-attachments/assets/303c9f5a-02c3-498b-8e43-c7f39e467175" />

**Key Findings**
- This segment includes 331 churned customers and 346 retained customers, corresponding to a 48.9% churn rate.
- Customers with medium account balances (€100k–150k) generate the highest churned balance (€55.81M) and show a churn rate of 57.27%.
- Mid-term customers (3–5 years) account for the largest churned balance (€24.91M) with a churn rate of 47.60%.
- Customers with low annual salaries (<€70k) tend to exhibit higher churn than higher-income customers within the same balance group.
- Long-term customers without additional banking products continue to demonstrate elevated churn risk.

**Business Implications**
Retention campaigns should focus on mid-career customers in Germany, particularly those maintaining medium account balances. Increasing product usage and strengthening customer engagement could significantly reduce churn.

## High-Risk Segment 3 – Male Customers Aged ≥51 ##
This dashboard analyzes churn patterns among mature male customers to identify behavioral and financial characteristics associated with customer attrition.
<img width="1414" height="950" alt="image" src="https://github.com/user-attachments/assets/dce3a3b0-9fea-470c-b87c-ff5307d81002" />

**Key Findings**
- This segment contains 244 churned customers and 413 retained customers, resulting in a 37.1% churn rate.
- Customers without a credit card experience an exceptionally high churn rate of 80.30%, highlighting weak product engagement.
- High-balance customers (>€150k) still exhibit a relatively high churn rate (36.51%), particularly in Germany.
- Germany continues to present the highest churn risk among all three countries for this segment.
- Customers with poor or fair credit scores generally show higher churn than customers with stronger credit profiles.

**Business Implications**
Cross-selling additional banking products, especially credit cards, should become a key retention strategy for mature male customers. Relationship management for high-value customers is also recommended.

## High-Risk Segment 4 – Customers Aged 41–50 Without Credit Cards ##
This dashboard investigates customers aged 41–50 who do not own a credit card, revealing how product adoption, gender, and account balance influence churn.
<img width="1404" height="946" alt="image" src="https://github.com/user-attachments/assets/73c97397-66ae-4eda-a037-d757c4156e5b" />

**Key Findings**
- This segment consists of 303 churned customers and 553 retained customers, representing a 35.4% churn rate.
- Female customers exhibit a significantly higher churn rate (41.65%) than male customers (29.89%).
- Customers with high account balances (>€150k) still experience substantial churn (46.88%), suggesting that financial value alone does not guarantee retention.
- In France, customers with medium account balances (€100k–150k) contribute the largest churned balance (€19.31M).
- The absence of a credit card remains one of the strongest indicators associated with customer churn.

**Business Implications**
Increasing product adoption through credit card campaigns and personalized offers should be prioritized for this segment. Female customers aged 41–50 represent an important target group for retention and cross-selling initiatives.

# Final Conclusion & Recommendations #
<img width="1678" height="974" alt="image" src="https://github.com/user-attachments/assets/275909de-33e0-46d3-bd02-de79d6b3d41f" />

This project successfully answered the key business questions by identifying the main drivers of customer churn, uncovering AI-generated high-risk customer segments, and providing actionable retention strategies. Through EDA, data modeling, and interactive Power BI dashboards, the solution enables stakeholders to monitor churn performance, understand customer behavior, and make data-driven retention decisions.
