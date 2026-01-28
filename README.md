## Assessing Financial Assets Behavioural Factors and Forecasting 

The study examines how behavioural sentiment factors influence financial asset
movements and evaluates multiple forecasting models to predict short-term
future behaviour of the S&P 500 index.

---

## 1. Project Objective

Financial asset prices are driven by both quantitative market dynamics and
behavioural factors such as investor sentiment. The objective of this project
is twofold:

1. To evaluate and compare traditional statistical, machine learning, and deep
   learning models for financial time-series forecasting.
2. To assess the role of behavioural sentiment indicators—derived from textual
   data—in explaining and supporting observed market movements.

The project integrates forecasting models with sentiment analysis outputs and
presents the results through interactive visual analytics.

---

## 2. Forecasting Models Implemented

The following forecasting approaches are applied to S&P 500 price data:

- **ARIMA** (statistical baseline)
- **Linear Regression** (baseline regression model)
- **XGBoost** (tree-based machine learning model)
- **LSTM** (deep learning model for sequential data)

The LSTM model is further used to generate multi-step forecasts for the next
few trading days.

---

## 3. Behavioural Sentiment Analysis

To capture behavioural factors, two sentiment analysis techniques are used:

- **VADER**  
  A lexicon-based sentiment model applied to textual financial data.

- **FinBERT**  
  A transformer-based language model fine-tuned on financial corpora, used for
  contextual sentiment classification.

Sentiment outputs are aggregated and aligned with market data to study their
relationship with asset price movements.

---

## 4. Python Files Description

- **01_S&P500_Forecasting.ipynb**  
  Data fetching, cleaning, exploratory analysis, statistical testing, and
  forecasting using ARIMA, Linear Regression, XGBoost, and LSTM. Includes
  short-horizon future forecasts using the LSTM model.

- **02_SentimentAnalysis_VADER.ipynb**  
  Behavioural sentiment extraction using the VADER lexicon-based approach,
  aligned with S&P 500 market data.

- **03_SentimentAnalysis_FinBERT.ipynb**  
  Financial sentiment analysis using FinBERT, including aggregation of article-
  level sentiment into daily indicators.

All notebooks are executed in Google Colab and export their outputs as CSV
files for downstream analysis.

---

## 5. Power BI Dashboard

A Power BI dashboard is developed using the processed CSV outputs generated
from the Python analysis. The dashboard provides interactive visualisations of:

- Market price trends
- Forecasting results
- Behavioural sentiment indicators
- Relationships between sentiment and price movement

A static preview image is included for reference.

---

## 6. Technologies Used

- Python (Pandas, NumPy, Scikit-learn, Statsmodels)
- TensorFlow / Keras
- XGBoost
- Natural Language Processing (VADER, FinBERT)
- Google Colab
- Power BI

---

## 7. Notes

- This repository is intended strictly for **academic research purposes**.
- Forecasting outputs and inferred signals are experimental and should not be
  interpreted as financial or investment advice.

---

## Author

**Pranjal Lalit Chavle**  
MSc Data Science
250062333


results/
├── model_comparison_metrics.csv
└── lstm_future_forecasts.csv
