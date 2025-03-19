# Tesla Stock Price Prediction using Linear Regression

## Project Overview
This project uses **machine learning** to analyze and predict **Tesla's stock price** based on historical data. It focuses on **predicting the next day's closing price** using **Linear Regression**. Project uses recent data from 2020-2025

## Project Steps
- Data collection and preprocessing
- Exploratory data analysis
- Feature engineering
- Data splitting
- Training the model
- Evaluation
- Visualization
- Conclusion
- Notes on debugging

## Dataset
We use **Yahoo Finance** to get Tesla's stock price from **2020-01-01 to 2025-03-13**.

The dataset includes:
- `Open`, `High`, `Low`, `Close` prices
- `Volume` of stocks traded
- **Feature created**: `Previous_Close` (shifted closing price)

## Machine Learning Model
- **Model Used**: `LinearRegression` from `sklearn`
- **Feature Used**: `Previous_Close`
- **Target Variable**: `Close`
- **Data Split**: 80% Train, 20% Test (no shuffling to preserve time sequence)

## Results
- The model predicts the next day's closing price based on the previous day's close with relatively close accuracy.
- Performance is assessed using standard metrics (e.g., MSE, MAE, RMSE).

## Installation & Library Usage
### 1. Install Dependencies
```bash
pip install yfinance pandas scikit-learn matplotlib seaborn
```

### 2. Run the Notebook
Execute `TSLA_ML_proj.ipynb` in Jupyter Notebook or Google Colab.

## Future Improvements
- Adding **more features** (e.g., moving averages, trading volume).
- Experimenting with **advanced models** (e.g., LSTMs for time series).

## Author
Created by [Danny DeSantiago] as part of a **machine learning portfolio project**.
