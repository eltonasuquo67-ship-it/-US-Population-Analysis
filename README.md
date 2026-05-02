# 📊 US State Population Analysis (1950–2015)

![Status](https://img.shields.io/badge/Status-Completed-green)
![Tools](https://img.shields.io/badge/Tools-Excel%20%7C%20SQL%20%7C%20Power%20BI-blue)
![Focus](https://img.shields.io/badge/Focus-Data%20Analysis-orange)

---

## 📌 Project Overview
This project analyzes population trends across different US states from 1950 to 2015.  
The goal is to identify growth patterns, compare states, and visualize demographic changes using data analysis tools.

---

## 🎯 Objectives
- Clean and structure US state population dataset  
- Analyze population growth across states and years  
- Compare population distribution between regions  
- Build interactive visualizations using Power BI  
- Generate insights for demographic trends  

---

## 🛠️ Tools & Technologies
- 📊 Microsoft Excel (Data Cleaning & Preparation)  
- 🗄️ SQL (Data Querying & Analysis)  
- 📈 Power BI (Dashboard & Visualization)  

---
## 📊 Dashboard Preview

![image alt](https://github.com/eltonasuquo67-ship-it/-US-Population-Analysis/blob/752d88cfecf76552b84aa800460cfaac13e80ff5/IMG_8204.png)


## 📊 Key Insights
- California and Texas show the highest population growth  
- Southern and Western states experienced faster expansion  
- Some Northern states showed slower growth or stability  
- Population shift increased toward urbanized states  

---

## 📁 Project Structure
``` id="g2n8ks"
US-State-Population-Analysis/
│
├── data/
│   └── us_population.csv
├── images/
│   └── dashboard.png
├── sql_queries.sql
├── powerbi_dashboard.pbix
└── README.md


## 🗄️ SQL Analysis

The dataset was analyzed using SQL to extract insights about population growth trends across US states.

### 📊 Key SQL Queries Used


-- Total population growth by state
SELECT 
    state,
    (MAX(population) - MIN(population)) AS total_growth
FROM state_population
GROUP BY state
ORDER BY total_growth DESC;




-- Population trend over time
SELECT 
    year,
    SUM(population) AS total_population
FROM state_population
GROUP BY year
ORDER BY year;



### 🔍 What this analysis shows
- Identifies states with the highest population growth  
- Shows overall population trend across years  
- Helps compare regional development patterns  
