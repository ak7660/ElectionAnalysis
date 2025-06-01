# Demographic Determinants of U.S. Presidential Election Outcomes  
### A County-Level Analysis of the 2020 Vote  
 **Date:** May 2025  

## Overview

This project investigates how county-level demographic variables influence U.S. presidential election outcomes, using the 2020 election as a case study. We integrate data from the 2020 U.S. Census, the American Community Survey (ACS), and historical election records to model and visualize the relationship between demographic patterns and voting behavior.

## Key Objectives

- Analyze the influence of variables like age, income, education, and race on vote outcomes.
- Develop both linear and logistic regression models to explain:
  - Vote share of the winning candidate (continuous outcome)
  - Likelihood of a Republican county-level win (binary outcome)
- Explore predictive limitations and diagnostic insights.

## Methods

### Data Sources
- **Demographic Data:** U.S. Census (2020), ACS
- **Election Data:** MIT Election Lab, U.S. House of Representatives archives

### Analysis Pipeline
- **Data Merging:** Joined on FIPS codes at the county level
- **EDA:** Visualized distributions by winning party using histograms and boxplots
- **Modeling:**
  - **Linear Regression:** Vote share of the winner
  - **Logistic Regression:** Probability of Republican win
- **Diagnostics:** Residual plots, Q-Q plots, ANOVA, confidence intervals

## Notable Findings

- Counties with older, more male populations tended to support the winning candidate more strongly.
- Higher proportions of white residents and lower college education were strongly associated with Republican wins.
- Despite significant coefficients, the linear model had a low explanatory power (Adj. R² ≈ 3.1%), suggesting other factors—like ideology or turnout—also play a key role.

## Limitations

- Ecological fallacy from county-level aggregation
- Omitted variables (e.g. ideology, turnout, campaign intensity)
- Potential multicollinearity among racial proportion predictors
- Cross-sectional data limited to 2020

## Future Work

- Include campaign, turnout, and political affiliation data
- Test non-linear and interaction effects
- Apply time-series and spatial models (e.g. GWR)
- Incorporate machine learning approaches



