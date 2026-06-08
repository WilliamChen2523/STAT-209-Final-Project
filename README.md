# STAT-209-Final-Project
# Strait of Hormuz Disruption Analysis: Oil Prices, Energy Security, and Regional Vulnerability

## Project Overview

The Strait of Hormuz is one of the world's most important energy transportation corridors, carrying a significant share of global crude oil and liquefied natural gas exports. Any prolonged disruption to shipping through the Strait has the potential to affect global energy markets, increase transportation costs, and create substantial economic uncertainty.

This project investigates the potential impacts of a Strait of Hormuz disruption on:

* Brent crude oil prices
* Energy market dynamics
* Government policy responses
* Regional energy vulnerability

The analysis combines exploratory data analysis (EDA), data visualization, and machine learning techniques to examine how shipping disruptions and market conditions influence oil prices.

---

## Research Questions

1. How might a disruption in the Strait of Hormuz affect Brent crude oil prices?
2. Which variables are most strongly associated with oil price fluctuations?
3. Which regions are most vulnerable to energy supply disruptions?
4. How have governments responded to energy-related crises?

---

## Datasets

### 1. Strait of Hormuz Shipping Dataset

* 125 observations × 26 variables
* Shipping activity
* Oil throughput
* LNG throughput
* Vessel attacks
* Insurance costs
* Brent crude oil prices

### 2. U.S. Gasoline Prices Dataset

* 50 observations × 9 variables
* State-level gasoline prices
* Fuel price changes following market disruptions

### 3. European Energy Policy Dataset

* 41 observations × 19 variables
* Government subsidies
* Price controls
* Energy support programs

### 4. Asia Energy Vulnerability Dataset

* 22 observations × 16 variables
* Oil import dependency
* Fuel affordability
* Refinery capacity
* Energy subsidies

---

## Methods

### Exploratory Data Analysis

* Descriptive statistics
* Correlation analysis
* Time-series visualization
* Regional comparisons

### Predictive Models

* Linear Regression
* Random Forest
* XGBoost

Model performance was evaluated using:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² (Coefficient of Determination)

---

## Key Findings

### Oil Market Dependence

Asia is the largest destination for oil transported through the Strait of Hormuz, making the region particularly vulnerable to supply disruptions.

### U.S. Fuel Price Impacts

Western U.S. states recorded the highest gasoline prices, while several southern and central states experienced the largest percentage increases following energy market disruptions.

### Model Performance

| Model             |    R² |
| ----------------- | ----: |
| Linear Regression | 0.965 |
| XGBoost           | 0.945 |
| Random Forest     | 0.827 |

Linear Regression achieved the strongest predictive performance, suggesting that the relationships within the dataset are largely linear.

### Feature Importance (XGBoost)

The most influential predictor of Brent crude oil prices was:

* `days_since_closure` (99.4% importance)

This finding suggests that market expectations and the duration of the disruption were more important than individual shipping indicators in explaining oil price movements.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost



## Future Work

Potential extensions include:

* Incorporating real-world shipping data
* Scenario-based forecasting under different disruption durations
* Additional geopolitical risk indicators
* Advanced time-series forecasting models

---

## Author

William

STAT 209 Final Project

University of California, Riverside



The datasets link:
1)https://www.kaggle.com/datasets/alitaqishah/iran-war-oil-shock-2026-brent-and-gas-tracker
2)https://www.kaggle.com/datasets/hussnainmamoon1/hormuz-shipping-crisis-2026-daily-dataset
3)https://www.kaggle.com/datasets/zkskhurram/world-vs-asia-fuel-prices
4)https://www.bruegel.org/dataset/2026-european-energy-crisis-fiscal-response-tracker
