# C02 Forecasting in R using Prophet
This project applies **time series forecasting** in R to predict future atmospheric C02 concentrations using the **Prophet** library.

The goal is to show how forecasting models can capture **trend and seasonality** in time series data.

## Project Overview
 - Dataset: Built-in R dataset `co2` (monthly atmospheric CO2 from Mauna Loa Observatory, 1958–1997)
 - Model: **Meta Prophet** for time series forecasting  
- Key Steps:
  1. Prepare the dataset (`ds` = time, `y` = CO2 levels)  
  2. Fit a Prophet forecasting model  
  3. Create a future dataframe (quarters ahead)  
  4. Forecast and visualize results

## Results
- The forecast shows a **continuing upward trend** in CO2 concentration  
- Seasonal pattern detected:
  - Increase in **spring (April–May)**  
  - Decline in **autumn (Sept–Oct)**  
- Prophet outputs include:
  - Forecast plot (actual vs predicted values)  
  - Trend + seasonality components

## Forecast Plot 
Here is the CO2 forecast generated using Prophet:

![CO2 Forecast](Results/CO2Forecast.png)

## Forecast Components
Trend and seasonality of the CO2 forecast:

![CO2 Trend & Seasonality](Results/C02Forecast2.png)

## How to Run
1. Clone this repo  
2. Open `co2_forecast.R` (or `.Rmd`) in RStudio  
3. Install dependencies:
   ```r
   install.packages(c("prophet", "zoo"))

   ```
