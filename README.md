# DDS-8555 Assignment 2: Build Regression Models  
**Student:** Abigail Albury-Bloom  
**Course:** DDS-8555 Predictive Analysis  
**Instructor:** Dr. Mohammad Yavarimanesh  
**Date:** November 9, 2025  

---

## 📄 Overview
This project analyzes the Abalone dataset to predict the age of abalone based on physical characteristics using two regression models:
- **Lasso Regression** (linear, regularized)
- **Random Forest Regressor** (nonlinear ensemble)

The analysis compares both models using Root Mean Squared Error (RMSE) and identifies the most important features influencing abalone age.

---

## 🧠 Methodology
- Preprocessed categorical and numerical data using `OneHotEncoder` and `StandardScaler`
- Split dataset 80/20 for training and validation
- Evaluated model performance with RMSE
- Verified regression assumptions (linearity, independence, normality, multicollinearity)
- Visualized top predictors using Random Forest feature importance

---

## 📊 Results

**Table 1. RMSE Comparison Between Lasso and Random Forest Models**

| Model              | RMSE   |
|--------------------|--------|
| Lasso Regression   | 2.1566 |
| Random Forest      | 2.0635 |

The Random Forest model achieved the lowest RMSE, indicating slightly higher predictive accuracy compared to the Lasso model.

### Top Predictors Identified by Random Forest
The Random Forest model ranked the following features as most important in predicting abalone age:

1. Shell weight  
2. Height  
3. Diameter  
4. Whole weight  
5. Length  

These variables contribute most to model accuracy, reflecting the strong biological relationship between physical size and the number of rings (age).

---

## 📂 Files in Repository
- `AlburyBloomADDS8555-2_RS.ipynb` – Jupyter Notebook containing full code, RMSE table, and feature importance summary  
- `Albury-BloomADDS8555-2_RS.docx` – Written report formatted in APA 7th edition  
- `AlburyBloomADDS8555-2_RS.pdf` – PDF version of the written report  
- `submission_lasso.csv` – Kaggle submission output for Lasso Regression model  
- `submission_rf.csv` – Kaggle submission output for Random Forest model  

---

## 🧩 Environment
Developed in Python 3.10 using the following libraries:
- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`
- `statsmodels`

---

## 🔗 Kaggle Competition
**Regression with Abalone Dataset**  
[Kaggle Link](https://www.kaggle.com/competitions/playground-series-s4e4)

---

## 🧾 References
Harrell, F. E. (2015). *Regression modeling strategies* (2nd ed.). Springer.  
James, G., Witten, D., Hastie, T., & Tibshirani, R. (2021). *An introduction to statistical learning* (2nd ed.). Springer.  
Kutner, M. H., Nachtsheim, C. J., & Neter, J. (2004). *Applied linear regression models* (4th ed.). McGraw Hill.
