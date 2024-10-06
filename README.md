# Yulu Business Case Study: Hypothesis Testing

## Overview

This project focuses on analyzing data from **Yulu**, India’s leading micro-mobility service provider, offering shared electric vehicles. Yulu aims to understand the factors affecting the demand for its shared electric bikes in various seasons, weather conditions, and days (holidays vs. working days).

The study includes:
- Exploratory Data Analysis (EDA)
- Statistical Hypothesis Testing
- Business Recommendations

## Project Scope

Yulu has experienced a dip in revenues and has engaged in consulting services to analyze and determine the factors impacting the demand for bike rentals. Specifically, this study aims to identify:
- How demand varies across **seasons** and **weather conditions**.
- Whether there is a significant difference in bike rentals on **holidays** vs. **working days**.
- Which conditions are most optimal for bike deployment and marketing strategies.

## Dataset Overview

The dataset used in this study contains the following columns:
- `datetime`: Timestamp of the bike rental
- `season`: Season (Spring, Summer, Fall, Winter)
- `holiday`: Whether the day is a holiday
- `workingday`: Whether the day is a working day
- `weather`: Weather condition (Clear, Cloudy, Rainy, etc.)
- `temp`: Temperature (Celsius)
- `atemp`: Apparent temperature (Celsius)
- `humidity`: Humidity percentage
- `windspeed`: Wind speed (m/s)
- `casual`: Count of casual users
- `registered`: Count of registered users
- `count`: Total count of bike rentals

## Methods and Techniques

### Exploratory Data Analysis (EDA)

The dataset was explored to understand key features and patterns in the data, including:
- **Seasonal trends** in bike rentals.
- **Impact of weather conditions** on demand.
- **Correlation** between temperature, humidity, and windspeed with bike usage.
- **Outlier detection** for rentals during holidays, working days, and weather conditions.

### Statistical Hypothesis Testing

Several hypothesis tests were conducted to validate the observed trends:
- **Two-Sample T-Test**: To analyze the difference in bike rentals between working days and holidays.
- **ANOVA (Analysis of Variance)**: To evaluate if the demand differs significantly across multiple weather conditions and seasons.
- **Levene's Test**: For checking homogeneity of variances before ANOVA.
- **Kruskal-Wallis Test**: Non-parametric test to validate the ANOVA results, given that the data is not normally distributed.

### Key Statistical Findings
1. **No Significant Difference** in bike rentals between holidays and working days.
2. **Weather Conditions**: Significant difference in demand across different weather conditions, with clear weather leading to higher rentals.
3. **Seasonal Influence**: Demand varies significantly across seasons, with summer showing the highest rental activity.

## Strategic Business Recommendations

Based on the findings, several strategic recommendations were provided to Yulu:
1. **Focus on Peak Rental Months**: Allocate resources and deploy more bikes during peak months (June, July, August).
2. **Dynamic Pricing Strategy**: Adjust bike rental prices based on weather and season to maximize profits.
3. **Targeted Marketing Campaigns**: Promote Yulu's services during summer and incentivize rentals during off-peak months.
4. **Optimize Bike Deployment**: Plan bike availability based on weather forecasts and ensure adequate supply during favorable conditions.
5. **Leverage Technology**: Invest in infrastructure and app enhancements to improve user experience and foster loyalty.

## Project Structure

```
├── data
│   └── bike_sharing.csv            # The dataset used in the analysis
├── notebooks
│   └── yulu-business-case-study.ipynb         # Jupyter notebook containing the EDA and hypothesis testing
├── README.md                       # Project documentation
```

## Results and Insights

The analysis results were conclusive in identifying the following insights:
- **Weather** and **Season** are the most influential factors affecting bike rental demand.
- **Holidays** and **Working Days** show no significant difference in demand.
- Targeting **summer** and clear weather conditions for marketing efforts will boost revenue.

## Conclusion

This study provides Yulu with actionable insights to drive better resource allocation, marketing strategies, and pricing mechanisms to enhance bike rental demand and revenue.
