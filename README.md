# Bellabeat Smart Device Analysis (SQL | BigQuery)
![SQL](https://img.shields.io/badge/SQL-BigQuery-blue)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)


Análisis SQL de datos de dispositivos inteligentes Fitbit con BigQuery para generar información de marketing para Bellabeat.
Bellabeat Case Study – SQL Analysis (BigQuery)
 Project Overview

This project analyzes smart device usage data to generate strategic marketing recommendations for Bellabeat.

The analysis was conducted using SQL in Google BigQuery and is based on publicly available Fitbit user data.

Business Problem

Bellabeat aims to grow in the global smart device market.
The objective of this analysis is to:

Identify trends in smart device usage

Segment users based on activity levels

Provide data-driven marketing recommendations

Dataset

Source: Kaggle

Dataset: FitBit Fitness Tracker Data

File used: dailyActivity_merged.csv

Sample size: 30 Fitbit users

Dataset Limitations

Small sample size (30 users)

Data not recent

May not represent global smart device users

Tools Used

SQL

Google BigQuery

Aggregations

CASE statements

CTEs

User segmentation

Date formatting and grouping

 Data Cleaning & Preparation

The following steps were performed:

Verified table structure and data types

Removed inconsistencies in date formatting

Created derived table (activity_cleaned)

Generated new variables:

day_of_week

activity_level (Sedentary, Moderately Active, Active)

Example transformation:

CASE
  WHEN TotalSteps < 5000 THEN 'Sedentary'
  WHEN TotalSteps BETWEEN 5000 AND 9999 THEN 'Moderately Active'
  ELSE 'Active'
END AS activity_level
 Exploratory Data Analysis
 User Activity Segmentation

Average daily steps by segment:

Sedentary → 1,633 steps

Moderately Active → 7,238 steps

Active → 13,444 steps

Most users fall into the Moderately Active segment.

 Weekly Activity Pattern

The lowest average step count occurs on:

Tuesday → 4,915 steps

This suggests a mid-week drop in physical activity.

 Key Insights

The majority of users do not reach the 10,000-step benchmark.

There is a significant behavioral gap between sedentary and active users.

Tuesday shows the lowest engagement level.

Moderate users represent the greatest opportunity for growth.

 Strategic Recommendations

Based on the findings, the following recommendations are proposed for Bellabeat:

 1. Progressive Goal Setting

Implement dynamic and personalized step goals instead of fixed 10,000-step targets.

 2. “Tuesday Boost” Campaign

Deploy targeted mid-week motivational notifications and activity challenges.

 3. Segment-Based Marketing Strategy

Develop differentiated engagement strategies for:

Low activity users

Moderate users

High activity users

 Business Impact

This analysis demonstrates how behavioral data can inform:

Personalized engagement strategies

Retention-focused marketing

Data-driven segmentation
Product feature development

Conclusion
The analysis reveals actionable patterns in user behavior that can support strategic growth initiatives. By leveraging activity segmentation and behavioral timing insights, Bellabeat can enhance user engagement and optimize its marketing strategy.

## 🔮 Future Improvements

- Incorporate sleep data for deeper behavioral insights  
- Apply window functions to analyze user trends over time  
- Develop a dashboard in Looker Studio  
- Expand dataset with larger sample size for better representativeness

## 👤 Author

Sergio Andres Garcia Peña  
Data Analyst | SQL | BigQuery  

### 📊 Weekly Activity Visualization (R)

![Weekly Steps](screenshots/weekly_steps.png)
