# Weather Impact on Sales at Blue Chip Café

## Overview

This project analyzes the effect of weather variables (temperature and precipitation) on the sales performance of the Blue Chip Café. Using historical weather and customer frequency data, the project predicts total annual revenue for the café, providing insights into how weather influences customer behavior and revenue generation.

## Problem Statement

The goal is to predict Blue Chip Café's total annual revenue for 2024 based on:
- Historical weather data (temperature and precipitation)
- Customer visit frequency data

## Key Features

- **Predictive Model**: Developed a mathematical model to calculate the café's daily customer count as a function of temperature and precipitation.
- **Revenue Estimation**: Simulated annual revenue by integrating customer spending patterns with weather-based customer frequency predictions.
- **Sensitivity Analysis**: Explored the impact of varying model assumptions, including spending patterns and weather sensitivities.
- **Visualizations**: Plots and histograms to illustrate findings, including revenue distributions and customer behavior trends.

## Methodology

1. **Data Collection**: Weather data from Vancouver and customer frequency data from Blue Chip Café.
2. **Assumptions**:
   - Customer count is influenced solely by temperature and precipitation.
   - Spending per visit is uniformly distributed between the menu's minimum and maximum prices.
3. **Model**:
   - Daily customer count: \( C(T, P) = \max\{C_0 + a(T - T_0) - b(P - P_0), 0\} \)
     - \( C_0 \): Reference customer count
     - \( T_0, P_0 \): Reference temperature and precipitation
     - \( a, b \): Sensitivity coefficients
4. **Simulations**: Monte Carlo simulations to estimate annual revenue.

## Results

- **Mean Revenue**: Predicted mean revenue with specified assumptions is $481,049.
- **Assumption Sensitivity**:
  - Changing spending range from $1.25–$12.50 to $7.50–$15.00 increases mean revenue to $787,388.
  - Modifying weather sensitivity coefficients affects revenue by 9–15%.
- **Probability Analysis**:
  - There is a 52.94% probability of exceeding the mean revenue of $481,049 under current assumptions.

## Visualizations

The project includes:
- Customer spending distribution.
- Revenue distribution with Kernel Density Estimate (KDE) plots.
- Hourly customer frequency trends.

## Technologies Used

- Python (NumPy, Pandas, Matplotlib, SciPy)
- Jupyter Notebook for simulations and visualizations
