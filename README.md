# Bank-Marketing-Analysis

## Overview
Used the data gotten from potential customers to answer different questions using SQL and added my insights.

## Tools Used
SQL, Excel

## Data Source
This data was gotten from kaggle [download here] (https://www.kaggle.com/datasets/yukeshmarudhasalam/bankmarketing)

## SQL Queries

## 1. Marital status and type of job

### 1a. What type of job did the married people do
``` SQL
SELECT job as "Type of Job", COUNT(marital) as "Number of Married People"
FROM Bank
WHERE marital = 'married'
GROUP BY "Type of Job"
ORDER BY COUNT(Marital) DESC;
```
