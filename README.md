# 🌍 Climate Change Temperature Analysis

This project explores historical climate change by analyzing Earth’s surface temperature trends from 1750 to 2024. It combines Python-based data analysis, Streamlit for interactive dashboards, and Tableau for visual storytelling.

![Climate-Change-Temperature-Analysis](https://github.com/user-attachments/assets/f33f04af-e71f-4a75-9ba9-d72da948969a)

🔹 Problem Statement

Climate change is one of the most pressing issues of our time. Rising global temperatures have significant impacts on ecosystems, economies, and human health. By analyzing long-term temperature datasets, we can better understand trends, seasonality, and country-level variations.

Goal: Perform exploratory data analysis (EDA) on global land temperature data, visualize trends, and build an interactive dashboard for storytelling.

🔹 Dataset

- Source: Berkeley Earth / Kaggle – Global Land Temperatures by Country

- Timeframe: 1750 – 2015

- Features:

- dt → date

- AverageTemperature

- AverageTemperatureUncertainty

Country

🔹 Approach

1. Data Cleaning

- Removed missing/unreliable early records (pre-1850)

- Handled missing temperature values with rolling means

- Aggregated data by year and country

2. Exploratory Data Analysis (EDA)

- Global average temperature trends over 250+ years

- Country-level warming rates (e.g., India vs USA vs Europe)

- Seasonal variation patterns

- Trend decomposition → long-term trend vs seasonality (using STL)

3. Visualization

- Time-series plots (global warming trend)

- Heatmaps (temperature anomalies by decade & country)

- Country ranking (warming rate °C/decade)

- Interactive dashboard in Streamlit/Tableau

🔹 Results

- 🌡 Global warming trend: Global land temperature has increased by ~1.2°C since the late 19th century.

- 📈 Acceleration: Warming has sharply accelerated since 1950.

- 🌍 Country differences: Northern hemisphere countries (e.g., Russia, Canada) show higher warming rates than equatorial regions.

- 📊 Seasonality: Winters are warming faster than summers in many regions.

🔹 Visualizations
Global Warming Trend


Heatmap of Temperature Anomalies


Country Ranking




🔹 Tech Stack

- Python: pandas, numpy, matplotlib, seaborn, statsmodels

- Visualization: Tableau, Streamlit

- Time-series decomposition: statsmodels.tsa.seasonal.STL

🔹 How to Run
git clone https://github.com/FnuAbhijith/Climate-Change-Temperature-Analysis.git
cd Climate-Change-Temperature-Analysis
pip install -r requirements.txt
streamlit run app.py
