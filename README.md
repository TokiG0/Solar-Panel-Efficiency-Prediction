# Solar-Panel-Efficiency-Prediction
<h1 align="center">☀️ Solar Panel Efficiency Prediction</h1>
<p align="center">
  <i>Submission for the Zelestra X AWS ML Ascend Challenge - 2nd Edition</i><br>
  <b>High-accuracy predictive modeling for solar panel efficiency</b>
</p>

---

## 📘 Overview

This project applies a structured machine learning pipeline to forecast solar panel efficiency using environmental and operational data. The final model leverages ensemble learning and advanced feature engineering to achieve high predictive accuracy.

---

## 🧰 Tools & Technologies

- **Language:** Python 3  
- **Environment:** Jupyter Notebooks (local setup)  
- **Libraries:**
  - Data Handling: `pandas`, `numpy`
  - Visualization: `matplotlib`, `seaborn`
  - Machine Learning: `scikit-learn`, `xgboost`, `lightgbm`, `catboost`, `optuna`

---

## 📊 Methodology

### 1. Data Preprocessing
- Cleaned missing/inconsistent values
- Removed outliers
- Scaled numerical features using `StandardScaler` / `MinMaxScaler`
- Encoded categorical variables

### 2. Feature Engineering
- Derived new features: power ratio, panel efficiency
- Created interaction features from temperature, irradiance, humidity
- Removed multicollinear and low-variance features

### 3. Model Development
- Baseline models: Linear Regression, Decision Trees
- Advanced models: XGBoost, LightGBM, CatBoost
- Final model: **Stacked Regressor** combining top-performing models
- Hyperparameter tuning via Grid Search and Optuna

### 4. Evaluation Strategy
- Metrics: RMSE, MAE, R² Score
- Validation: 5-Fold Cross-Validation
- Target: >90% accuracy on test data
- Leaderboard feedback used for iterative improvements

---

## 📁 File Mapping

| File Name                     | Description                                 |
|------------------------------|---------------------------------------------|
| `Solar_V2.ipynb`             | Intermediate enriched model development     |
| `solar_v1_accuracy_89.90197.ipynb` | First successful version with ~90% accuracy |
| `Solar_v3_tus (1).ipynb`     | Final stacked model with performance tuning |

---

## 🚀 Reproduction Steps

To reproduce the results locally:

### 1. Install dependencies

You can install all required packages using:

```bash
pip install matplotlib seaborn numpy pandas lightgbm xgboost scikit-learn catboost scipy optuna