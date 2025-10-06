## 🧠 Project Overview

This project is designed to analyze and forecast user financial data using advanced time series models and AI-powered tools.

### 🔹 Data Collection

We collect user transaction data directly from their bank statements.
(Imagine we have a secure connection with the bank — once the user adds their bank account, we can automatically fetch their transaction history.)

### 🔹 Transaction Categorization

We categorize transactions into different clusters using the DBSCAN clustering algorithm.

These clusters are then divided into income and expense categories.

### 🔹 Time Series Forecasting

The categorized transactions are fed into separate time series forecasting models to predict category-wise income and expenses for the next 30 days.

### 🔹 Account Balance Prediction

We use the N-BEATS model to predict account balances for the next 30 days.

The predicted balances are then fed into the TFT (Temporal Fusion Transformer) models for income and expense forecasting to improve overall accuracy.

### 🔹 Daily Expense Prediction

We also use two N-BEATS pipelines to predict daily total expenses.

These results are used as additional input features for the TFT models (income and expenses) to further enhance prediction accuracy.

### 🔹 Two-Stage TFT Model

Our TFT model for income and expense forecasting operates in two stages:

The first TFT predicts whether a transaction will occur or not.

The second TFT predicts the amount of the occurred transaction.

### 🔹 Model Selection

We use a combination of time series forecasting models such as TFT (Temporal Fusion Transformer) and N-BEATS.

These models were selected after careful analysis and experimentation with various time series forecasting techniques.

![image_alt](https://github.com/Kalindu-C/bankingApp/blob/main/Model%20Selection.PNG)

### 🤖 Agentic Chatbot

Additionally, we provide an agentic financial chatbot that allows users to ask questions about their finances.

The chatbot is built using open-source models to ensure data privacy and security.

![image_alt](https://github.com/Kalindu-C/bankingApp/blob/main/Agent%20Architecture.PNG)

#### Here is high level architecture of our application

![image_alt](https://github.com/Kalindu-C/bankingApp/blob/main/Architecture.PNG?raw=true)
