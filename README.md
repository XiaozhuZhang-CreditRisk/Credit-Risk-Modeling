# Credit Risk Analytics

## Overview
This repository implements several credit risk modeling techniques commonly used in banking and financial risk management, including:

- Probability of Default (PD) modeling
- Time series credit risk analysis
- Portfolio default simulation (Vasicek model)
- Machine learning approaches for credit risk classification

The project demonstrates a full credit risk modeling workflow from driver analysis to portfolio risk simulation.

---

## Project Structure

### 1. Wholesale PD Model (`01_Wholesale_PD_Model.ipynb`)
Traditional PD estimation using financial ratios and neural networks. Focuses on identifying key financial drivers of default.

<p align="center">
  <img src="https://github.com/user-attachments/assets/996fbd47-4a9e-4ee4-b4dc-daf1372758a0" width="700" alt="Neural Network PD Model Architecture">
  <br>
  <em>Figure 1: Neural Network Architecture for Wholesale PD Estimation</em>
</p>

### 2. Time Series Model (`02_Time_Series_Model.ipynb`)
Time series analysis of default rates and macroeconomic risk drivers to understand cyclical risk patterns.

### 3. Default Simulation & Measurement (`03_Default_Simulation_and_Measurement.ipynb`)
Monte Carlo simulation of default rates using the Vasicek single-factor credit model to estimate portfolio loss distributions.

<p align="center">
  <img src="https://github.com/user-attachments/assets/1b2f9c65-4e73-4200-8e4a-baca68726f63" width="700" alt="Vasicek Model Simulation Results">
  <br>
  <em>Figure 2: Portfolio Loss Distribution via Vasicek Model</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/c76fad86-cc60-4df5-a0de-4ca523afce65" width="700" alt="Asset Correlation Sensitivity Analysis">
  <br>
  <em>Figure 3: Sensitivity Analysis of Asset Correlation Parameters</em>
</p>

### 4. ML PD Model (`04_ML_PD_Model.ipynb`)
Advanced machine learning methods for PD prediction and credit risk classification, including comparative case studies against traditional models.

---

## Methodology

The models apply several quantitative techniques standard in the industry:

- **Neural Networks**: For non-linear PD estimation.
- **GroupKFold Cross-Validation**: Specifically designed to prevent firm-level data leakage.
- **Financial Ratio Analysis**: Identifying robust risk drivers (e.g., profitability, leverage).
- **Vasicek Model**: Asymptotic single-factor model for portfolio risk.
- **Monte Carlo Simulation**: Generating thousands of scenarios for stress testing.
- **Model Evaluation**: Using AUC (Area Under Curve) and KS (Kolmogorov-Smirnov) statistics.

---

## Key Results

- **Best Performance**: The optimal PD model achieved an **AUC = 0.90** using a parsimonious 3-variable financial driver combination.
- **Key Drivers**: Profitability ratios showed the strongest negative correlation with default probability.
- **Portfolio Calibration**: Simulation suggests an asset correlation (ρ) ≈ 0.1 best matches observed default volatility in the dataset.
- **ML Advantage**: Machine learning models successfully captured complex, non-linear relationships between financial variables that linear models missed.

---

## Tech Stack

- **Languages**: Python
- **Data Manipulation**: NumPy, Pandas
- **Machine Learning**: Scikit-learn, TensorFlow / Keras
- **Statistical Analysis**: SciPy
- **Visualization**: Matplotlib

---

## Author

**Xiaozhu Zhang**  
M.S. Enterprise Risk Management, Columbia University  
*Focus: Risk Management, Credit Risk Modeling & Risk Consulting*
