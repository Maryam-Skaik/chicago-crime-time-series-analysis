# 🚔 Chicago Crime Time Series Analysis (2001–2022)

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458.svg)
![TimeSeries](https://img.shields.io/badge/Time%20Series-Analysis-orange.svg)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen.svg)

---

## 📌 Project Overview

This project analyzes **Chicago crime data from 2001 to 2022** using time series techniques.  
The goal is to extract meaningful insights about crime trends, seasonal behavior, geographic distribution, and holiday effects.

The analysis is designed as part of a data science portfolio project focusing on:

- Time series exploration
- Data aggregation and resampling
- Feature engineering
- Visualization and pattern discovery

---

## 🎯 Objectives

The main objectives of this analysis are:

- Identify which police districts experience the highest and lowest crime rates
- Analyze long-term crime trends across years
- Explore crime behavior during major holidays
- Detect seasonal patterns and recurring cycles in crime data

---

## 📊 Dataset Description

The dataset contains **Chicago crime records reported between 2001 and 2022**, originally sourced from the Chicago Data Portal.

### Key Features:

- `Date` – Timestamp of the crime incident
- `Primary Type` – Category of crime (e.g., THEFT, BATTERY)
- `Description` – Detailed crime description
- `Location Description` – Type of location where crime occurred
- `District`, `Ward`, `Beat` – Administrative divisions
- `Arrest` – Whether an arrest was made
- `Domestic` – Whether the crime was domestic-related
- `Latitude`, `Longitude` – Geographic coordinates

📦 Total Records: **7,713,109**

---

## ⚙️ Technologies Used

- Python 🐍
- Pandas & NumPy
- Matplotlib & Seaborn
- Statsmodels (Time Series Decomposition)
- Holidays library (Feature Engineering)

---

## 🧹 Data Preparation

Key preprocessing steps include:

- Combining yearly CSV files into a single dataset
- Converting `Date` column to datetime format
- Sorting and indexing by time
- Handling missing values in spatial and categorical features
- Removing unnecessary columns (`ID`)
- Creating a **daily crime count time series**

---

## 📈 Exploratory Analysis

### 🏢 1. Police District Analysis

We analyzed crime distribution across districts for 2022.

**Findings:**
- Crime is highly uneven across districts
- Some districts show significantly higher crime concentration than others

---

### 📉 2. Crime Trends Over Time

We evaluated yearly crime totals from 2001 to 2022.

**Findings:**
- Overall crime shows a **long-term decreasing trend**
- Sharp decline observed after 2010
- Temporary fluctuations exist in recent years

We also analyzed individual crime categories:

- Theft, burglary, and battery show strong declines
- Motor vehicle theft shows recent increases
- Some violent crimes remain relatively stable

---

### 🎉 3. Holiday Crime Patterns

We examined crime behavior during major US holidays.

**Findings:**
- Highest crime activity occurs during:
  - New Year’s Day
  - Independence Day
  - Labor Day
- Common crimes during holidays include:
  - Battery
  - Theft
  - Criminal damage

📌 Insight: Holidays tend to increase social activity, which correlates with higher crime rates.

---

### 🔄 4. Seasonality Analysis

We applied **time series decomposition** using a 12-month period.

**Findings:**
- Crime data exhibits a clear **yearly seasonal cycle**
- Seasonal effects repeat consistently every 12 months
- Magnitude of variation is moderate but consistent

### 📊 Cycle Characteristics:
- Cycle length: **12 months**
- Variation range: approximately **-5,400 to +3,480 crimes**
- Seasonality is present but weaker than long-term trend

---

## 📌 Key Insights Summary

- 📉 Crime in Chicago has decreased significantly over two decades
- 🏢 Crime distribution is uneven across police districts
- 🎉 Holidays are associated with spikes in criminal activity
- 🔄 Strong yearly seasonality exists in crime patterns
- ⚖️ Long-term trend dominates over seasonal fluctuations

---

## 🧠 Conclusion

This analysis demonstrates how time series techniques can uncover meaningful patterns in large-scale crime data.

By combining statistical decomposition and feature engineering, we can better understand:

- How crime evolves over time
- When crime is most likely to increase
- Where crime is most concentrated

These insights can support better decision-making for public safety planning and resource allocation.
