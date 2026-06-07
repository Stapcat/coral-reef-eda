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

**Dataset:** 1,073 observations of class Anthozoa (corals & anemones) 
from 9 countries, sourced from GBIF citizen science records (2022–2024).

**1. Geographic distribution**
Observations are concentrated in tropical and subtropical zones,
consistent with known coral reef biogeography. The Indo-Pacific
region (Australia, Philippines, Indonesia, Fiji, Maldives) shows
strong representation. The Coral Triangle (Philippines, Indonesia)
is clearly visible as a biodiversity hotspot on the map.

**2. Species composition**
The most observed species are sea anemones (*Anthopleura sola*,
*Entacmaea quadricolor*, *Radianthus magnifica*), not hard corals.
This likely reflects observer bias — anemones are visually striking
and frequently photographed by divers. The first true hard coral
appears at position 4 (*Galaxea fascicularis*).

**3. Seasonality**
After removing a data artifact (January default dates), February,
March and May emerge as peak observation months. This reflects
diving seasons in the Southern Hemisphere (Australia, Fiji) where
summer runs December–February, and pre-monsoon periods in
tropical Asia where visibility is best in spring.

**4. Data quality note**
~43% of records had month=1, suggesting missing date metadata
defaulting to January. This highlights an important limitation of
citizen science data that should be considered in any downstream
analysis. After exclusion, all 12 months are represented in the
remaining dataset.

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
