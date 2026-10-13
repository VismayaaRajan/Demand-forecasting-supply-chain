# Demand Forecasting for Supply Chain Optimization Using Historical Sales Data

## Problem Statement
This project uses historical retail sales data to develop a predictive model for forecasting daily sales and supporting supply chain planning.

## Dataset
Store Sales – Time Series Forecasting dataset from Kaggle, containing sales records and supporting store, holiday, and oil-price information.

Dataset: https://www.kaggle.com/competitions/store-sales-time-series-forecasting

## Methodology
1. Data loading and understanding
2. Data preprocessing and feature engineering
3. Exploratory Data Analysis (EDA)
4. Integration of supporting datasets
5. Random Forest Regression
6. Model evaluation using MAE and RMSE
7. Feature importance and result interpretation

## Results
- Random Forest MAE: 78,460.90
- Random Forest RMSE: 119,450.47
- Seven-day lag baseline MAE: 108,539.92

## Tools Used
Python, Pandas, Matplotlib, Scikit-learn, Google Colab.

## How to Run
1. Download the notebook from this repository.
2. Open it in Google Colab.
3. Download the dataset files from Kaggle.
4. Upload the required CSV files to Colab.
5. Run the notebook cells in order.

## Note
The model predicts total daily sales aggregated across stores and product families. The reported results are from the project's chronological test split.
