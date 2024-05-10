# Business Case: Yulu - EDA & Hypothesis Testing




## About Yulu
Yulu is India’s leading micro-mobility service provider, which offers unique vehicles for the daily commute. Starting off as a mission to eliminate traffic congestion in India, Yulu provides the safest commute solution through a user-friendly mobile app to enable shared, solo and sustainable commuting.

Yulu zones are located at all the appropriate locations (including metro stations, bus stands, office spaces, residential areas, corporate offices, etc) to make those first and last miles smooth, affordable, and
convenient!
## Problem Statement
Yulu has experienced significant revenue dips recently and has contracted a consulting company to understand the factors affecting demand for shared electric cycles in the Indian market.

The company wants to know:
* Which variables are signi cant in predicting the demand for shared electric cycles in the Indian market?
* How well those variables describe the electric cycle demand
## Column Profiling

| Variables | Description |
| :- | :- |
| datetime  | date-time |
| season 1 | spring |
| season 2 | summer |
| season 3 | fall |
| season 4 | winter |
|  holiday | whether day is a holiday or not |
|  workingday | if day is neither weekend nor holiday is 1, otherwise is 0. |
| weather 1 | Clear, Few clouds, partly cloudy, partly cloudy|
| weather 2 | Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist |
| weather 3 | Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds |
| weather 4 | Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog |
| temp | temperature in Celsius |
| atemp | feeling temperature in Celsius |
| humidity | humidity |
| windspeed | wind speed |
| casual | count of casual users |
| registered | count of registered users |
| count | count of total rental bikes including both casual and registered |




## Analysis Steps

### Exploratory Data Analysis (EDA):
1. Exploring Data
* Checked dataset structure, data types, and dimensions.
* Checked missing values in each column.
* Statistical Summary of the data.
2. Univariate Analysis
* Used Histogram for Univariate Analysis of all Continuous Variables.
* Performed Univariate Analysis of Categorical Variables using count plot.
3. Bivariate Analysis
* Generated heatmap to Analyse relation between Continuous Variables
* Analyzed relation between Categorical Variables ('season', 'holiday', 'workingday', 'weather') using heatmap.

### Hypothesis Testing:
1. T - Test to check if Working Day has an effect on the number of electric cycles rented:
* Performed Visual Analysis, Hypothesis Formation, Test Assumptions.
* checked Test Assumptions Using 1. Statistical method 2. Visual Analysis
* T-statistic and p-value were calculated to evaluate the significance of the difference.


2. Anova to check if No. of cycles rented is similar or different in different Weather
* Performed Visual Analysis, Hypothesis Formation, Test Assumptions.
* checked Test Assumptions Using 1. Statistical method 2. Visual Analysis
* F-statistic and p-value were calculated to assess the significance of differences across groups.

3. Anova to check if No. of cycles rented is similar or different in different Season
* Performed Visual Analysis, Hypothesis Formation, Test Assumptions.
* checked Test Assumptions Using 1. Statistical method 2. Visual Analysis
* F-statistic and p-value were calculated to assess the significance of differences across groups.

4. Chi-square test to check if Weather is dependent on the season
* Used Contingency Table for Analysis of Weather vs Season 
* Formulated Hypothesis and Checked Test Assumptions Using both Statistical and Visual Analysis.
* Chi-square statistic and p-value were computed to determine the dependence between weather and season.
