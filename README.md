# NYPD Shooting Incident Data Report: Victim's Perspective

*Author: Helios SL So | University of Colorado Boulder | Master of Science in Data Science | June 2023*

---

## 📌 Overview

This project explores the **NYPD Shooting Incident Data (Historic)** from [NYC Open Data](https://data.cityofnewyork.us/Public-Safety/NYPD-Shooting-Incident-Data-Historic-/833y-fsy8), offering a **victim-centered perspective** on shooting incidents in New York City from 2006 to the end of the last calendar year.

We analyze trends by **borough**, **victim's age group**, and **victim's sex group**, and build a **Poisson regression model** to forecast future cases. Visualizations and model limitations are discussed, and potential **biases in data interpretation** are acknowledged.

---

## 📊 Data Source

- **URL:** [NYC Open Data Portal - NYPD Shooting Incident Data](https://data.cityofnewyork.us/Public-Safety/NYPD-Shooting-Incident-Data-Historic-/833y-fsy8)
- **Agency:** New York Police Department (NYPD)
- **Last Updated:** April 27, 2023
- **Rows:** 27.3K+  
- **Columns:** 26  
- **Time Span:** 2006 – latest full calendar year

---

## 🛠 Tools & Technologies

- **Language:** R
- **Environment:** RStudio
- **Libraries:** `tidyverse`, `ggplot2`, `dplyr`, `tidyr`, `knitr`

---
## 📈 Key Analyses

### 1. Exploratory Data Analysis (EDA)

- Trends of shooting cases by **borough** over **year-month**
- Breakdown by **victim age groups** and **sex**
- Identification of **peak months** and **vulnerable demographics**

### 2. Modeling

- **Poisson Regression** to model the number of shooting cases by:
  - Borough
  - Year
  - Victim Age Group

- **Forecast** shooting cases for 2024–2028
- Visualize **actual vs. predicted** values

### 3. Bias Assessment

- Observational bias (e.g., interpreting drops during COVID-19)
- Lack of causal explanation for trend changes

---

## 📉 Observations

- **Brooklyn** and **Bronx** consistently report the highest number of shootings.
- Cases declined slightly before and during **COVID-19**, then surged post-pandemic.
- Victims are mostly aged **25–44**, followed by **18–24**.
- **Male victims** are significantly more common.
- **Summer months** show more incidents across boroughs.

---

## ⚠ Limitations

- Regression model fit was poor — future predictions show divergence from past trends.
- Poisson regression may be overly simplistic for this data — consider time series models (e.g., ARIMA, Prophet) or advanced ML methods for better performance.
- Predictions assume stationarity and ignore external factors (policy, policing, social shifts).

---
## 📚 References

-  NYC Open Data - NYPD Shooting Data
-  Generalized Linear Models in R – DataCamp
-  Regression Analysis in R – GeeksforGeeks
-  Bias in Research – Scribbr
