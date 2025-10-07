## Solar-Power-Generation-Forecasting-in-Smart-Cities
Solar power forecasting using Random Forest, SVR, CNN, CNN-LSTM, and Seq2Seq models on the BigML dataset. Models evaluated with MSE, RMSE, MAE, R². SHAP used for explainable AI to interpret feature impact and improve smart city solar energy prediction accuracy.

#### Overview
This repository contains a complete data science pipeline for forecasting solar power generation using time-series and weather data. The project applies explainable machine learning, including classical models and deep learning, to achieve high-accuracy predictions and interpretable results.[1]

#### Dataset
- The dataset (`BigML_Dataset_5f50a4cc0d052e40e6000034.csv`) features chronological measurements including temperature, wind, humidity, sky cover, daylight, barometric pressure, and actual solar power generated for each time interval.
- Feature engineering includes temporal lags, normalization, and encoding for robust forecasting.
- Target column is “Power Generated,” referenced against multivariate weather and timing data.[2]

#### Code Structure
- Jupyter/Python notebook and `.py` implementations are provided for full workflow.
- Main file: Data loading, exploration, preprocessing (imputation, encoding, scaling), feature engineering, chronological splitting, training, evaluation, and visualization.
- Key models used: Random Forest, Support Vector Regressor, CNN, CNN-LSTM, Seq2Seq Encoder-Decoder LSTM.
- The code includes implementation of SHAP and LIME for explainable AI, hyperparameter tuning, feature importance, and comparative evaluation.[1]

#### Workflow Steps
- Load and explore dataset, visualizing distributions and correlations.
- Time-series feature creation and handling lags.
- Data normalization and one-hot encoding of categorical variables.
- Chronologically safe train/validation/test splits for realistic time-series forecasting.
- Train and evaluate multiple models including Random Forest, SVR, CNN, CNN-LSTM, and Seq2Seq LSTM.
- Assess performance with metrics (MSE, RMSE, R^2) and visualize Predictions vs Actuals.
- Interpret model predictions using explainable AI (SHAP, LIME), partial dependence plots, and feature attribution analyses.
- Results are visualized across short, medium, and long forecasting horizons.[1]

#### Usage Instructions
1. Clone the repository and ensure all dependencies are installed (Python, pandas, numpy, scikit-learn, matplotlib, seaborn, tensorflow, keras, SHAP, LIME).
2. Place the dataset file in the working directory.
3. Run the main code file or notebook (`SolarPower.ipynb` or equivalent).
4. Follow cells sequentially for: data preparation, feature engineering, model training, validation, performance reporting, and explanation.
5. Visual results and tables will output key insights on solar power prediction and feature impact.

#### Requirements
- Python 3.6+
- pandas, numpy, scikit-learn, tensorflow, keras, matplotlib, seaborn, SHAP, LIME
- Jupyter Notebook or compatible IDE

#### Results & Explainability
- Models are compared by predictive accuracy and interpretability.
- SHAP and LIME are used to analyze which weather/timing variables most influence solar power output.
- Visualizations show actual vs predicted power and feature impact, supporting actionable insights for smart city optimization.
