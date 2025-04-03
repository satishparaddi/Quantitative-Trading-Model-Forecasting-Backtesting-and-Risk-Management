# 📊 Quantitative Trading Model: Forecasting, Backtesting, and Risk Management

## 📌 Overview

This project presents a data-driven approach to stock market forecasting and risk analysis by leveraging deep learning and statistical techniques. Specifically, we employ a Long Short-Term Memory (LSTM) neural network to predict stock prices and generate actionable insights. The model is enhanced with Monte Carlo simulation for risk assessment and includes backtesting for evaluating trading strategies.

---

## 🔧 Key Features

- 📉 **LSTM-based Time Series Forecasting**: Predicts future stock prices based on historical trends.
- 📈 **Technical Analysis Indicators**: Uses 100-day and 200-day moving averages to detect trends.
- 🔁 **Backtesting**: Simulates trades using historical predictions to evaluate strategy performance.
- 🎲 **Monte Carlo Simulation**: Models a range of possible price outcomes and evaluates risk.
- 🧾 **User Parameters**: Enables users to select stocks and forecast duration with actionable insights.

---

## 📁 Files

- `Stock_prediction_&_Risk_Management.ipynb`: Jupyter Notebook containing the full implementation.
- `Project_Report.pdf`: PDF report explaining the methodology, experiments, and results.
- `README.md`: This documentation file.

---

## 🛠️ Methodology

### 1. 📥 Data Collection
- Collected using `yfinance` API from Jan 1, 2010 to Dec 7, 2024.

### 2. 🧹 Data Preprocessing
- Used `MinMaxScaler` to normalize closing price values.
- Created 60-day time windows to train the LSTM for next-day prediction.

### 3. 🧠 Model Architecture
- Two LSTM layers with dropout for regularization.
- One Dense layer for prediction.
- Optimizer: Adam; Loss function: Mean Squared Error (MSE).

### 4. 🏋️ Training and Evaluation
- 80% of the data used for training, 20% for testing.
- Trained over 100 epochs with a batch size of 32 and a 10% validation split.

### 5. 🔁 Backtesting
- Evaluated model-generated buy/sell signals on historical data to analyze profitability.

### 6. 🛡️ Risk Management
- Incorporated Monte Carlo simulation to simulate thousands of possible future price paths.
- Quantified risk and variability in investment outcomes.

---

## 📈 Results

- LSTM model generated reasonably accurate short-term forecasts.
- Moving averages and LSTM-based signals were backtested successfully.
- Monte Carlo simulations provided probabilistic forecasting for risk insight.

---

## 🎯 Conclusion

This project highlights the value of combining LSTM models with statistical simulations and traditional technical indicators for trading. Enhancements in model tuning, additional features, and live deployment could further improve accuracy and usability.

---

## 🛠 Technologies Used

- Python
- TensorFlow / Keras
- NumPy, Pandas
- Matplotlib, Seaborn
- Scikit-learn
- yFinance
- Jupyter Notebook

---
