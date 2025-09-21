# Analysis of Air Quality in India (2015-2020)

## 📌Objective
This project is an exploratory data analysis (EDA) of a large-scale air quality dataset from various cities across India. The primary goal is to clean, analyze, and visualize pollution trends to uncover key insights about geographical hotspots and seasonal patterns for major air pollutants.

## 📂Dataset
The data was sourced from Kaggle and includes daily and hourly readings for pollutants such as PM2.5, PM10, AQI, etc., from multiple monitoring stations across India spanning from 2015 to 2020.

## ❓Key Questions & Insights

This analysis answers several key questions about air quality in India:

* **Which regions are the most polluted?**
    * There is a significant **geographical disparity** in air quality. Cities in the **Indo-Gangetic Plain** (like Gurugram, Delhi, and Patna) consistently show the highest PM2.5 levels.

* **How does pollution change with the seasons?**
    * A strong **seasonal pattern** was identified across the country. Pollution levels consistently peak during the **Winter** months and are at their lowest during the **Monsoon**.

* **What is the scale of the pollution difference?**
    * The analysis reveals a massive gap between regions, with the most polluted cities having average PM2.5 levels **over four times higher** than the least polluted cities (e.g., Delhi vs. Aizawl).

## ⚙️Methodology

1.  **Data Cleaning:** Missing time-series data was handled using a **forward-fill (`ffill`)** and **backward-fill (`bfill`)** strategy to ensure data integrity without skewing the results.
2.  **Data Preparation:** Merged multiple data sources (`city_day`, `station_day`, `stations`) to create comprehensive datasets for analysis.
3.  **Feature Engineering:** Created `Season` and `Month` columns from datetime objects to enable temporal analysis.
4.  **Analysis & Visualization:** Used `pandas` for data manipulation and aggregation, and `matplotlib`/`seaborn` to create clear visualizations that communicate the findings.

## Tools Used
* Python 🐍
* Pandas 🐼
* Matplotlib & Seaborn 📊
* Jupyter Notebook 📓
