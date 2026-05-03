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


## 📊 Key Insights

🇺🇸 Regional Distribution of States

* West: 13 states (26%)
* Midwest: 12 states (24%)
* South: 16 states (32%)
* Northeast: 9 states (18%)

➡️ The South region dominates, containing nearly one-third of all US states.

⸻


## 📈 Population Growth Trend (Example: California)

* 1950: ~10M
* 2015: ~39M
* Growth: +290% increase

➡️ States like California show consistent long-term growth, driven by economic opportunities and migration.

⸻


## 🌍 Overall Population Trend

* All states show a steady upward trend from 1950–2015
* Growth accelerates significantly after the 1980s

➡️ Indicates national population expansion and urbanization trends

⸻


## 🏙️ State-Level Contribution

* High population states dominate the total trend (e.g., California, Texas, Florida)
* Smaller states contribute less but show steady growth patterns

➡️ Population distribution is uneven, with a few states driving national totals.

⸻


## 📊 Census Region Breakdown

The dataset categorizes states into:

* Midwest
* Northeast
* South
* West

➡️ Enables regional comparison and segmentation analysis



## 🛠️ Tools & Technologies
- 📊 Microsoft Excel (Data Cleaning & Preparation)  
- 🗄️ SQL (Data Querying & Analysis)  
- 📈 Power BI (Dashboard & Visualization)  

---
## 📊 Dashboard Preview

![image alt]( 


## 📊 Observations
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


 🗄️ SQL Analysis

The dataset was analyzed using SQL to extract insights about population growth trends across US states.

📊 Key SQL Queries Used


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
