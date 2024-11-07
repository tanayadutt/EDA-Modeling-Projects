# EDA/Modeling Projects

# Walmart Sales Analysis and Forecasting

This project explores and analyzes the Walmart store sales dataset to gain insights into sales trends, seasonal patterns, and the impact of external factors. The analysis includes statistical modeling and time series forecasting to better understand the dataset.

## Project Overview

The goals of this project are to:
1. Analyze trends in Walmart sales over time.
2. Identify the impact of holidays on sales.
3. Understand the influence of external factors (CPI, fuel prices, temperature, and unemployment).

## Dataset

- **Source**: Walmart store sales dataset
- **Key Columns**:
  - `Store`: Store ID
  - `Date`: Date of the sales record
  - `Weekly_Sales`: Weekly sales amount
  - `Holiday_Flag`: Indicator for holiday weeks
  - `Temperature`: Average temperature for the week
  - `Fuel_Price`: Fuel price in the area
  - `CPI`: Consumer Price Index
  - `Unemployment`: Unemployment rate

## Analysis and Insights

### 1. Holiday Impact on Sales
Overall, results highlight the influence of holiday periods on sales increases, regardless of temperature, fuel prices, CPI, or unemployment variations. This trend could be useful for forecasting and promotional planning, as it suggests that certain weeks may consistently yield higher sales, particularly around known holiday periods.

### 2. External Factors Impacting Sales
Explored how external factors like fuel price, CPI, and unemployment influence weekly sales through correlation analysis and linear regression models.

### 3. Store with the highest Sales and Year of hughest sales.
Performed a seasonal decomposition on weekly sales to separate the data into trend, seasonality, and residual components, revealing underlying patterns in sales cycles.

## Modeling

### 1. Linear Regression
The MSE is high, it suggests that the model's predictions have significant error and may be poorly aligned with actual sales, which might indicate missing influential variables or a need for more complex modeling.

### 2. KMeans Clustering
Applied KMeans clustering to segment stores based on sales behavior, grouping similar stores together and identifying patterns among different clusters.

### 3. ARIMA Time Series Forecasting
Developed an ARIMA model to forecast future weekly sales, providing predictions based on past data trends and seasonal adjustments.

## Repository Structure

```plaintext
├── data/                   # Raw dataset and any data preprocessing steps
├── notebooks/              # Jupyter Notebook with analysis and model code
├── images/                 # Generated plots and visuals
└── README.md               # Project documentation
