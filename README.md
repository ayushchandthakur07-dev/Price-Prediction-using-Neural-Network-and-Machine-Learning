# Price Prediction with Ensemble and Hybrid Neural Models 📈

This repository contains a Statistics Project titled "Price prediction using Neural Network,". It explores the application and comparison of advanced machine learning models to forecast the stock price of Apple Inc. (AAPL).

## 📝 Overview

The primary goal of this project is to implement and evaluate various sophisticated models for financial time-series forecasting by leveraging historical stock data, this analysis compares the effectiveness of an ensemble method (Random Forest) against hybrid deep learning architectures (CNN-LSTM and LSTM with Attention) in capturing complex market dynamics.The dataset consists of daily AAPL stock data from **2013 to 2023**, sourced via the `yfinance` library.

---

## 📊 Models Implemented

This repository showcases my work on the following three models:

1.  **Random Forest:** A robust ensemble learning method that builds multiple decision trees to capture non-linear relationships and is resilient to overfitting.Feature engineering includes lagged prices, rate of change (ROC), volume trends, and calendar features.
2.  **Hybrid CNN-LSTM:** A hybrid architecture that uses Convolutional Neural Networks (CNNs) to identify localized patterns (like volatility clusters) and Bidirectional LSTMs to model temporal dependencies, providing a comprehensive view of market data.
3.  **LSTM with Attention Mechanism:** An enhancement of the traditional LSTM network. The attention mechanism allows the model to dynamically assign more weight to significant historical time steps, improving prediction accuracy and interpretability, especially during volatile periods.

---

## ✨ Features

-   **Advanced Feature Engineering:** Created features like lagged prices, moving averages (MA44, MA7, MA21), momentum, rate of change (ROC), and volatility to enrich the input data.
-   **Model Comparison:** Rigorous evaluation using standard regression metrics to compare the predictive power of different architectures.
-   **Robust Preprocessing:** Utilized `StandardScaler` for the CNN-LSTM model and `RobustScaler` for the LSTM with Attention model to handle outliers effectively.
-   **Hyperparameter Optimization:** Employed Bayesian optimization for the Random Forest model to find the best-performing parameters.

---

## 🛠️ Technology Stack

-   **Python 3.x**
-   **TensorFlow:** For building the CNN-LSTM and LSTM with Attention models.
-   **Scikit-learn:** For the Random Forest model, data preprocessing, and evaluation metrics.
-   **Pandas:** For data manipulation and analysis.
-   **NumPy:** For numerical operations.
-   **yfinance:** For downloading historical stock data.
-   **Matplotlib & Seaborn:** For data visualization.

---

### **Prerequisites**
Make sure you have Python 3.8+ installed on your system.

## 📈 Results & Performance

Here is a summary of the performance metrics for each model on the test dataset:

| Model | R² Score | MAE ($) | RMSE ($) |
| :--- | :---: | :---: | :---: |
| Random Forest | 0.8160 | 5.56 | 8.27 |
| CNN-LSTM Hybrid | 0.6844 | 7.60 | 9.74 |
| LSTM with Attention | 0.2733 | 12.16 | 14.75 |
  
   cd your-repo-name

