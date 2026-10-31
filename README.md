# Time-Series-Energy-Consumption-Forecasting-Trend-Analytics
A time-series forecasting and data science portfolio project designed to model, analyse, and interpret temporal fluctuations in total energy consumption using Python and statistical modelling techniques.

# Project Overview
This Jupyter Notebook contains a complete machine learning pipeline for time-series forecasting of electrical energy consumption. It downloads a multi-region energy dataset, merges and cleans the hourly records, aggregates the total energy load, and trains a Long Short-Term Memory (LSTM) deep learning model using TensorFlow and Keras to predict future energy consumption trends.

<img width="1031" height="547" alt="image" src="https://github.com/user-attachments/assets/82aefcdc-f128-4a35-b11a-bab9aecead68" />

# Key Findings
1. The model's predicted values (orange dashed line) have flatlined at approximately 360,000 units, effectively predicting only the historical mean. It fails to capture any of the dynamic variance or seasonal peaks present in the actual dataset.
2. Actual energy consumption (blue line) exhibits severe volatility, fluctuating between 300,000 and 420,000 units. The model underestimates peak demand by up to 60,000 units (~14.3%) and overestimates troughs by roughly 50,000 units (~16.7%).
3. Whilst the training and validation loss curves converged to low values (~0.0003), this visual result proves the model suffered from underfitting/mode collapse due to over-smoothing or insufficient feature complexity.
4. Deploying this forecast in a real-world energy grid would lead to severe load-balancing failures—causing power deficits during unpredicted peak hours and over-generation during trough periods.
