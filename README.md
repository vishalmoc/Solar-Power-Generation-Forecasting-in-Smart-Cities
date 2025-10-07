

---

# Solar-Power-Generation-Forecasting-in-Smart-Cities ☀️🏙️

[![Python](https://img.shields.io/badge/Python-3.10-blue)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.15-orange)](https://www.tensorflow.org/)
[![Keras](https://img.shields.io/badge/Keras-2.15-red)](https://keras.io/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-1.3.0-green)](https://scikit-learn.org/)

Optimized forecasting of **solar power generation in smart cities** using classical and deep learning models, combined with **explainable AI (SHAP & LIME)** to interpret feature impacts and improve predictive accuracy.

---

## Project Overview

This project implements a **full data science pipeline** for forecasting solar power generation using **time-series weather data**. The workflow applies classical regression models, deep learning, and explainable AI to deliver **accurate and interpretable predictions**.

**Goal:** Predict solar power output accurately while understanding the influence of environmental and temporal factors.

---

## Dataset

* File: `BigML_Dataset_5f50a4cc0d052e40e6000034.csv`
* Features include: temperature, wind, humidity, sky cover, daylight, barometric pressure, and actual solar power generated.
* **Feature Engineering:** Temporal lags, normalization, encoding for robust time-series forecasting.
* **Target Column:** `Power Generated`

---

## Code Structure

* Jupyter Notebook and Python scripts provide the **complete workflow**:

  * Data loading & exploration
  * Preprocessing: imputation, encoding, scaling
  * Feature engineering and chronological splits
  * Model training, hyperparameter tuning, evaluation
  * Visualization and explainable AI (SHAP, LIME)

* **Key Models Used:**
  | Model | Description |
  |-------|-------------|
  | Random Forest | Ensemble tree-based regression for robust predictions |
  | SVR | Support Vector Regression for capturing non-linear trends |
  | CNN | Convolutional Neural Network for feature extraction from time series |
  | CNN-LSTM | Hybrid CNN and LSTM for temporal-spatial pattern learning |
  | Seq2Seq LSTM | Encoder-Decoder LSTM for multi-step time-series forecasting |

---

## Workflow Steps

1. Load dataset and explore distributions, correlations, and missing values.
2. Create time-series features and handle temporal lags.
3. Normalize numeric variables and one-hot encode categorical features.
4. Chronologically split data into train, validation, and test sets.
5. Train and evaluate models: Random Forest, SVR, CNN, CNN-LSTM, Seq2Seq LSTM.
6. Assess performance with **MSE, RMSE, MAE, R²**.
7. Interpret model predictions using **SHAP & LIME**, including partial dependence and feature attribution plots.
8. Visualize predictions for short-, medium-, and long-term forecasting horizons.

---

## Evaluation Metrics

| Metric | Description                                                            |
| ------ | ---------------------------------------------------------------------- |
| MSE    | Mean Squared Error, measures average squared prediction error          |
| RMSE   | Root Mean Squared Error, penalizes larger errors                       |
| MAE    | Mean Absolute Error, measures average absolute prediction error        |
| R²     | Coefficient of determination, measures variance explained by the model |

---

## Results & Explainability

* Compare predictive accuracy and interpretability across models.
* **SHAP & LIME** reveal which weather/timing features most influence solar power output.
* Visualizations include:

  * Predicted vs Actual Solar Power
  * Feature importance and impact plots
* Supports **actionable insights** for smart city energy management.

**Sample Visualization:**
*(Add plots here using Markdown: `![Predicted vs Actual](path_to_plot.png)`)*

---

## Installation & Usage

```bash
git clone https://github.com/your-username/Solar-Power-Generation-Forecasting-in-Smart-Cities.git
cd Solar-Power-Generation-Forecasting-in-Smart-Cities
pip install -r requirements.txt
jupyter notebook SolarPower.ipynb
```

* Follow notebook cells for **data preparation, feature engineering, model training, validation, evaluation, and explanation**.

---

## Requirements

* Python 3.6+
* pandas, numpy, scikit-learn, tensorflow, keras, matplotlib, seaborn, SHAP, LIME
* Jupyter Notebook or compatible IDE

---

## Contributing

Contributions are welcome! Open issues or submit pull requests to improve models, visualizations, or explanation techniques.

---

