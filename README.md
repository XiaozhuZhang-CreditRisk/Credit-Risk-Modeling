# Credit Risk Analytics

## Overview
This repository implements several credit risk modeling techniques commonly used in banking and financial risk management, including:

- Probability of Default (PD) modeling
- Time series credit risk analysis
- Portfolio default simulation (Vasicek model)
- Machine learning approaches for credit risk

The project demonstrates a full credit risk modeling workflow from driver analysis to portfolio risk simulation.

---

## Project Structure

**01_Wholesale_PD_Model.ipynb**  
Traditional PD estimation using financial ratios and neural networks.

**02_Time_Series_Model.ipynb**  
Time series analysis of default rates and macroeconomic risk drivers.

**03_Default_Simulation_and_Measurement.ipynb**  
Monte Carlo simulation of default rates using the Vasicek single-factor credit model.

**04_ML_PD_Model.ipynb**  
Machine learning methods for PD prediction and credit risk classification (including case studies).

---

## Methodology

The models apply several quantitative techniques used in credit risk modeling:

- Neural networks for PD estimation
- GroupKFold cross-validation to prevent firm-level data leakage
- Financial ratio based risk drivers
- Vasicek credit portfolio model
- Monte Carlo simulation
- AUC and KS statistics for model evaluation

---

## Key Results

- Best PD model achieved **AUC = 0.90** using a parsimonious 3-variable financial driver combination.
- Profitability ratios showed the strongest correlation with default probability.
- Portfolio simulation suggests **asset correlation ≈ 0.1** best matches observed default volatility.
- Machine learning models successfully capture non-linear relationships between financial variables and default risk.

---

## Tech Stack

- Python
- NumPy, Pandas
- Scikit-learn
- TensorFlow / Keras
- SciPy
- Matplotlib

---

## Author

**Xiaozhu Zhang**  
M.S. Enterprise Risk Management, Columbia University  
*Focus: Credit Risk Management & Quantitative Modeling*
