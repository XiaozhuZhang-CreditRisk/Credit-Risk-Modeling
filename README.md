# Credit Risk Modeling

This repository contains several credit risk modeling implementations developed in Python.  
The project focuses on **Probability of Default (PD) estimation, credit cycle modeling, and default rate simulation** using both traditional statistical methods and machine learning techniques.

The models were developed as part of credit risk analytics coursework and demonstrate practical implementations of risk modeling techniques widely used in banking and financial institutions.

---

# Project Structure

The repository includes four main modeling modules:

## 1. Wholesale PD Model

This notebook builds a **Probability of Default (PD) model for wholesale borrowers** using financial and firm-level data.

Main steps:

- Data loading and preprocessing
- Feature analysis
- Logistic regression modeling using `statsmodels`
- Model performance evaluation using **ROC-AUC**

Key libraries used:

- pandas
- statsmodels
- scikit-learn
- matplotlib

Purpose:

Estimate firm-level default probability and evaluate model discriminatory power.

---

## 2. Machine Learning PD Model

This notebook develops a **machine learning-based PD model** using a neural network architecture implemented with **TensorFlow / Keras**.

Main components:

- Data preprocessing
- Feature scaling using `StandardScaler`
- Cross-validation using `GroupKFold`
- Neural network model training
- Model evaluation using:
  - ROC-AUC
  - Log Loss

Key libraries:

- TensorFlow
- scikit-learn
- pandas
- numpy

Purpose:

Compare machine learning approaches with traditional statistical PD models and improve predictive performance.

---

## 3. Default Simulation and Measurement

This notebook models **portfolio default dynamics** using historical default rate data.

Main steps:

- Historical default rate analysis
- Estimation of mean and volatility of default rates
- Monte Carlo simulation of default rates
- Distribution analysis of simulated default outcomes

Key libraries:

- numpy
- pandas
- scipy
- matplotlib

Purpose:

Understand the distribution and variability of credit default rates under stochastic scenarios.

---

## 4. Time Series Credit Risk Model

This notebook analyzes **credit default rates using time series techniques**.

Main steps:

- Load credit portfolio default data
- Stationarity testing using **ADF test**
- Time series modeling using **ARIMA/SARIMA**
- Forecasting future credit risk trends

Key libraries:

- statsmodels
- pandas
- pandas_datareader
- matplotlib

Purpose:

Model macro credit cycles and forecast future default trends.

---

# Technologies Used

Python ecosystem:

- pandas
- numpy
- statsmodels
- scikit-learn
- TensorFlow / Keras
- scipy
- matplotlib

---

# Applications

These models demonstrate techniques used in:

- Credit risk modeling
- Probability of default estimation
- Credit portfolio risk measurement
- Default rate forecasting
- Machine learning applications in financial risk

---

# Author

Xiaozhu Zhang

M.S. in Enterprise Risk Management  
Columbia University

Fields of interest:

- Credit Risk Management
- Risk Control Strategy
- Risk Consult
