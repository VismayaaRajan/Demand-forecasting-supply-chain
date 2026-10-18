# Demand Forecasting for Supply Chain Optimization Using Historical Sales Data

## Problem Statement
This project uses historical retail sales data to develop predictive models for forecasting daily sales and supporting inventory management and supply chain planning. It compares multiple regression algorithms to identify the best-performing model based on forecasting error metrics.

## Datasets
**1. Store Item Demand Forecasting Challenge**

Contains historical sales records by date, store, and item.

Dataset: https://www.kaggle.com/competitions/demand-forecasting-kernels-only

**2. Rossmann Store Sales**

Contains historical store sales along with supporting information such as dates, promotions, customer counts, and holidays.

Dataset: https://www.kaggle.com/competitions/rossmann-store-sales

Both datasets are analysed independently and are not merged.

## Methodology
1. Data loading and understanding
2. Data cleaning and preprocessing
3. Exploratory Data Analysis (EDA)
4. Data transformation and feature engineering
5. Daily sales aggregation and lag feature creation
6. Regression model development using Linear Regression, Decision Tree, Random Forest, Gradient Boosting, and Extra Trees
7. Model evaluation using MAE, RMSE, WAPE, and R²
8. Model comparison, visualization, and result interpretation

The project follows the six stages of the KDD process: Selection, Data Cleaning, Transformation, Data Mining, Interpretation and Evaluation, and Knowledge Presentation.

## Results

**Store Item Demand Forecasting Challenge**
- Best model: Extra Trees Regressor
- MAE: 540.58
- RMSE: 898.45
- WAPE: 1.8349%
- R²: 0.980755

**Rossmann Store Sales**
- Best model: Extra Trees Regressor
- MAE: 724,880.89
- RMSE: 1,332,483
- WAPE: 10.9455%
- R²: 0.828052

Extra Trees Regressor achieved the best overall performance among the five tested models on both datasets in the project's chronological validation experiments.

## Tools Used
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Jupyter Notebook, Google Colab, Git, and GitHub.

## How to Run
1. Download the project notebook from this repository.
2. Open it in Jupyter Notebook or Google Colab.
3. Download both datasets from the Kaggle links above.
4. Place the CSV files in the locations specified in the notebook, or update the file paths.
5. Install the required Python libraries if needed.
6. Run the notebook cells in order to perform preprocessing, feature engineering, model training, evaluation, and visualization.

## Note
The experiments use daily aggregated sales rather than individual forecasts for every store-item combination. The reported metrics are based on a chronological validation split of the labelled training data, not the hidden official Kaggle test sets. Lag features may use actual previous sales observations during rolling validation, so the results should not automatically be interpreted as multi-day forecasts made entirely in advance. The two datasets have different sales scales, so their absolute error values should not be compared directly.

## Author
**Vismayaa Rajan**  
Symbiosis Institute of Technology, Nagpur  
Course: Predictive Analytics  
Academic Year: 2026
