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
<img width="289" height="180" alt="1" src="https://github.com/user-attachments/assets/4f6c7bef-4a48-4ec7-ab82-6b26a159072e" />


### 1b. What type of job did the single people do
``` SQL
SELECT job as "Type of Job", COUNT(marital) as "Number of Single People"
FROM Bank
WHERE marital = 'single'
GROUP BY "Type of Job"
ORDER BY COUNT(Marital) DESC;
```
<img width="295" height="180" alt="2" src="https://github.com/user-attachments/assets/130cbb4d-c654-444c-8743-8b5ee140f8e3" />

### 1c. What type of job did the divorced people do
``` SQL
SELECT job as "Type of Job", COUNT(marital) as "Number of Divorced People"
FROM Bank
WHERE marital = 'divorced'
GROUP BY "Type of Job"
ORDER BY COUNT(Marital) DESC;
```
<img width="310" height="179" alt="3" src="https://github.com/user-attachments/assets/1e404021-bfbf-4524-9ed4-24fdcecf4788" />

### INSIGHT
The married people did blue collar jobs the most, while the single and divorced did admin the most. The married people were also the most slef employed.

## Dashboard
<img width="1301" height="632" alt="4" src="https://github.com/user-attachments/assets/501b9493-ad59-4cb5-a821-6a78b4ff74d3" />

## 2. Level of education & type of job

### 2a. What type of job did people with basic.4y education do?

```SQL
SELECT job as "Type of Job", COUNT(education) as "Basic.4y Education"
FROM Bank
WHERE education = 'basic.4y'
GROUP BY "Type of Job"
ORDER BY COUNT(education) DESC;
```
<img width="269" height="181" alt="5" src="https://github.com/user-attachments/assets/d5204a43-0d88-4fd5-9acc-053b1c24d157" />

### 2b. What type of job did people with basic.6y education do?

```SQL
SELECT job as "Type of Job", COUNT(education) as "Basic.6y Education"
FROM Bank
WHERE education = 'basic.6y'
GROUP BY "Type of Job"
ORDER BY COUNT(education) DESC;
```
<img width="263" height="184" alt="6" src="https://github.com/user-attachments/assets/0a8204c2-35f6-4e06-a3d4-406b2e3d1d28" />
