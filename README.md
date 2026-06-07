# 🪸 Coral & Anemone Observations — Exploratory Data Analysis

An exploratory data analysis (EDA) of global coral and anemone 
observations using open citizen science data from GBIF.

## 📌 Project Goal
Practice data science skills on real ecological data while 
contributing to the open science community. Data was collected 
by citizen scientists and uploaded via platforms like iNaturalist.

## 📊 What's Inside
- Data loading from GBIF API using `pygbif`
- Data cleaning and quality assessment
- 4 visualizations:
  - Observations by country
  - Top 15 most observed species
  - Seasonality of observations (with data artifact detection)
  - Global geographic distribution map

## 🔍 Key Findings
- Sea anemones dominate the dataset, likely due to observer bias
- February and May are peak observation months
- 70% of records had a January default date — a data quality issue 
  common in citizen science datasets
- Observations are concentrated in tropical/subtropical zones

## 🛠️ Tools & Libraries
- Python 3
- pandas
- matplotlib
- pygbif (GBIF API client)
- plotly

## 📁 Data Source
[GBIF.org](https://www.gbif.org) — Global Biodiversity Information 
Facility, class Anthozoa (corals & anemones), 2024 records.

## 👤 Author
Beginner data scientist interested in marine ecology and open science.
