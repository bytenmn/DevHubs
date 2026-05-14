# Short-Term Stock Price Prediction

## Task Objective

Predict the next trading day's closing price using the current day's market data (Open, High, Low, Volume). The notebook demonstrates a simple supervised-learning workflow for short-term forecasting and compares a linear model with an ensemble tree-based regressor.

## Dataset Used

- Source: Historical daily stock data fetched from Yahoo Finance via the `yfinance` library.
- Example ticker used in the notebook: `AAPL` (Apple Inc.).
- Time span: 5 years of daily observations (configurable in the notebook).
- Columns used: `Open`, `High`, `Low`, `Close`, `Volume`. The target is the next day's `Close` (shifted by one day).

## Models Applied

- Preprocessing: sequential train/test split (earliest 80% training, latest 20% testing) and `StandardScaler` applied to features.
- Models trained and compared:
  - `LinearRegression` (ordinary least squares)
  - `RandomForestRegressor` (n_estimators=100, random_state=42)
- Evaluation metrics: RMSE (root mean squared error) and R² (coefficient of determination).

## Key Results & Findings

- The notebook prints RMSE and R² for each model on the held-out test period and visualizes actual vs predicted next-day close prices.
- Observational finding: `Random Forest` generally better captures nonlinear relationships and tends to outperform plain linear regression for this task and dataset.
- Limitations: the simple feature set (only same-day Open/High/Low/Volume) restricts predictive power; performance can vary by ticker and market regime.

## Recommendations & Next Steps

- Improve features: add lagged price/return features, technical indicators (moving averages, RSI, etc.), and date/time features.
- Use time-series aware validation (walk-forward or expanding-window cross-validation) when tuning hyperparameters.
- Experiment with stronger models: XGBoost/LightGBM, Prophet, or neural models (LSTM/Transformer) for sequence modeling.
- Consider modeling returns or predicting direction (classification) depending on downstream use.

## How to Run

1. Install dependencies (example):

```
pip install yfinance pandas numpy scikit-learn matplotlib seaborn
```

2. Open and run `Stock_Price_Prediction.ipynb` in this folder to reproduce results.

---
Generated from the `Stock_Price_Prediction.ipynb` notebook in this folder.
