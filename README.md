# Statistical Analysis of CPI and Income

## Overview
This project investigates the relationship between the Consumer Price Index (CPI) and Average Income in Canada using linear regression and bootstrap methods. The analysis aims to determine the correlation between these variables and examine income disparities between different provinces.

## Table of Contents
- [Overview](#overview)
- [Introduction](#introduction)
- [Datasets](#datasets)
- [Methods](#methods)
- [Guiding Questions and Visualizations](#guiding-questions-and-visualizations)
- [Results](#results)
- [Things to Note](#things-to-note)

## Introduction
The Income and Cost of day-to-day items are critical topics in today's news as they affect everyone. CPI and income, two variables selected for statistical analysis, offer valuable insights into economic trends and consumer spending patterns. The Consumer Price Index (CPI) represents changes in prices experienced by Canadian consumers. It measures price changes by comparing, through time, the cost of a fixed basket of goods and services (Statistics Canada, 2023).

As international students, effectively managing our money and rent are our main priorities in Canada. This research motivated us to analyze these specific datasets to understand the correlation between CPI and Average Income.

Throughout the last four decades, the price of goods has essentially been increasing, whereas the Average Income across Canada and provinces has also been rising, but not at the same rate as the CPI. Although CPI and Income are correlated, the statistical strength of this relationship is not well understood. Therefore, one objective of this project is to statistically determine the correlation between CPI and Average Income through linear regression and utilize the model to predict future average income based on theoretical future CPI values.

Additionally, we will compare the income means between four different provinces: Ontario (ON), British Columbia (BC), Nova Scotia (NS), and Prince Edward Island (PEI) to identify any income disparities.

## Datasets
We used two datasets in this report: 
1. **Income of Individuals by Age Group, Sex, and Income**: This dataset includes values for years ranging from 1976 to 2021, focusing on geography, age group, sex, income source, and various statistics.
2. **Consumer Price Index (CPI)**: This dataset includes annual average CPI values from 1914 to 2022, categorized into various sectors such as Food, Shelter, Household Operations, etc.

Both datasets are publicly available through the Statistics Canada website.

## Methods
### Linear Regression
To determine the correlation between CPI and Average Income, we used a linear regression model. We tested the following hypothesis:
- **Null Hypothesis (H0)**: There is no significant relationship between CPI and income.
- **Alternative Hypothesis (HA)**: There is a significant relationship between CPI and income.

### Bootstrap Methods
Bootstrap techniques were applied to estimate the accuracy of the correlation coefficient and to compare income means between provinces. We tested the following hypothesis for income disparities:
- **Null Hypothesis (H0)**: The difference between the two means is equal to 0.
- **Alternative Hypothesis (HA)**: The difference between the two means is NOT equal to 0.

## Guiding Questions and Visualizations

### Guiding Question 1 – Is CPI correlated with Average Income for Canada?
We created visualizations to examine the correlation between CPI and Average Income using scatter plots and linear regression lines. Additionally, we conducted a linear regression analysis and checked the model assumptions such as normality and homoscedasticity.

### Guiding Question 2 - Are there any income disparities between different provinces?
We compared the average income across selected provinces (ON, BC, NS, PEI) using bar plots and conducted statistical tests to determine if there are significant differences in income means between these provinces.

## Results

### Results for Guiding Question 1
- The R-squared value is 0.900, indicating a strong positive linear correlation.
- The correlation coefficient is 0.949.
- The p-value obtained is 2.2e^-16, suggesting a significant relationship between CPI and Income.
- Using the predict function, we estimated that when the CPI is at 200, the Average Income for Canadians will be in the range of 57181.51 to 63182.78.

### Results for Guiding Question 2
- The difference in average income for ON and BC is $3231.
- The difference in average income for NS and PEI is $6495.
- The difference in average income for ON and PEI is $16095.

Overall, there are statistically significant differences in income means between the provinces, indicating income disparity.

## Things to Note
- We treated the population data provided by Statistics Canada as sample data.
- The analysis focused on two variables: CPI and Average Income.
- We obtained a p-value of 2.2e^-16 for multiple tests, which is due to R's limit at that p-value, consistently supporting the alternative hypothesis.
