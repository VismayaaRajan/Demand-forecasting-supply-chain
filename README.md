# Demand Forecasting for Supply Chain Optimization Using Historical Sales Data

## 1. Problem Statement
Demand forecasting helps businesses estimate future product demand and sales using historical data. Inaccurate forecasts can lead to overstocking, stock shortages, and inefficient inventory management. This project develops and evaluates machine learning models to predict future demand and sales using historical sales patterns and relevant features.

## 2. Datasets
Two datasets were used and analyzed separately:

- **Store Item Demand Forecasting Challenge:** Historical daily sales data for individual store-item combinations from 2013 to 2017.
- **Rossmann Store Sales:** Historical daily sales data from Rossmann stores from 2013 to 2015, including store information and promotional details.

Sources:
- [Store Item Demand Forecasting Challenge](https://www.kaggle.com/competitions/demand-forecasting-kernels-only)
- [Rossmann Store Sales](https://www.kaggle.com/competitions/rossmann-store-sales)

## 3. Methodology and Approach
The project follows the Knowledge Discovery in Databases (KDD) process:

1. **Data Selection:** Loaded the two datasets and selected relevant sales, store, item, and date information.
2. **Data Cleaning:** Handled missing values and prepared the datasets for analysis.
3. **Data Transformation:** Extracted date-based features and created lag features and rolling statistics from historical sales. Promotional information was also used for the Rossmann dataset.
4. **Model Development:** Trained and compared five machine learning models: Linear Regression, Decision Tree, Random Forest, Gradient Boosting, and LightGBM.
5. **Model Evaluation:** Used chronological training and testing splits to evaluate forecasts using MAE, MSE, RMSE, WAPE, and R².
6. **Knowledge Presentation:** Compared model performance and visualized forecasts and feature importance to identify useful demand patterns.

## 4. Steps Followed
1. Loaded and explored both datasets independently.
2. Cleaned and preprocessed the data.
3. Created date, lag, and rolling-statistic features.
4. Split the data chronologically into training and testing sets.
5. Trained the five machine learning models.
6. Generated predictions for the test periods.
7. Evaluated and compared model performance using regression metrics.
8. Visualized actual versus predicted values and analyzed feature importance.
9. Identified the best-performing model for each dataset.

## 5. Results
LightGBM achieved the best overall performance on both datasets.

| Dataset | Best Model | MAE | RMSE | WAPE | R² |
|---|---|---:|---:|---:|---:|
| Store Item Demand | LightGBM | 5.87 | 7.61 | 10.75% | 0.9284 |
| Rossmann Store Sales | LightGBM | 555.9 | 808.4 | 7.97% | 0.9300 |

## 6. Tools and Technologies
- Python
- Pandas and NumPy
- Scikit-learn
- LightGBM
- Matplotlib and Seaborn
- Jupyter Notebook / Google Colab

## 7. Conclusion
The project demonstrates how machine learning can use historical sales patterns to forecast demand and support inventory planning and supply chain decisions. Among the models evaluated, LightGBM produced the strongest overall results on both datasets.
