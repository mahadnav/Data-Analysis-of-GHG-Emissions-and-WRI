# Data Analysis of GHG Emissions and WRI

## Introduction
I chose this project for my Data Science course at LUMS in Fall 2022. 

This notebook explores the relationship between greenhouse gas emissions, climate risk, and socioeconomic factors at a country level. The analysis aims to understand how emissions impact a country's vulnerability to climate-related risks, utilizing machine learning techniques and causal inference methods. Below is an overview of the notebook contents:

## 1. Libraries
Ensure you have installed the necessary libraries using pip:
```bash
pip install googletrans==4.0.0-rc1
```
The notebook utilizes the following libraries:
- `pandas` for data manipulation
- `numpy` for numerical computations
- `matplotlib` and `seaborn` for data visualization
- `sklearn` for machine learning models
- `statsmodels` for statistical analysis
- `googletrans` for translating country names

## 2. Data Cleaning
### 2.1 Importing Data
Three datasets are imported:
- `capital_cities.csv`: Contains information about capital cities.
- `greenhouse_emission.csv`: Includes greenhouse gas emission data.
- `world_risk_index.csv`: Provides the World Risk Index (WRI) data.

### 2.2 Data Merging and Cleaning
- Dataframes are merged based on country names and cleaned to remove null values and ensure consistency.
- String units are removed from emission values, and numerical values are converted to appropriate data types.

## 3. Exploratory Data Analysis (EDA)
### 3.1 Key Insights
- Countries with high WRI, vulnerability, lack of coping capabilities, and emissions are identified.
- Trends and relationships between variables are explored through bar plots and correlation matrices.

## 4. Machine Learning
### 4.1 Predictive Modeling
- Linear regression and random forest regression models are trained to predict WRI based on exposure, vulnerability, and susceptibility factors.
- Model performance is evaluated using Root Mean Squared Error (RMSE).

## 5. Causal Inference
### 5.1 Analysis
- Causal inference analysis is conducted to understand the impact of CO2 and Methane emissions per capita on WRI.
- Treatment variables are created based on emission levels, and the Average Treatment Effect (ATE) is calculated.
- Findings suggest a correlation between higher per capita emissions and lower WRI, possibly due to socioeconomic factors.

## Conclusion
This notebook provides detailed explanations, code snippets, and visualizations to explore the relationship between emissions and climate risk at a country level. The analysis offers insights into the complex interplay between environmental factors, socioeconomic conditions, and vulnerability to climate-related risks. Further research could delve deeper into causal mechanisms and policy implications arising from these findings.
