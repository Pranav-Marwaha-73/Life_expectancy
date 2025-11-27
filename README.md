# Life_expectancy

📈 Life Expectancy Prediction using Advanced Regression Models
🏷️ Machine Learning • Regression • XGBoost • Data Science
📝 Abstract

This project presents a machine learning–driven approach to accurately predict life expectancy using a comprehensive 15-year dataset from 193 countries (sourced from Kaggle).
The workflow includes:

Two-stage Exploratory Data Analysis (EDA)

Robust missing value imputation (Mean + kNN)

Categorical encoding

Benchmarking 40+ regression models using LazyPredict

Hyperparameter tuning for high-performing models

Final selection of XGBRegressor, achieving an exceptional R² of 96.87%

These results highlight the effectiveness of careful preprocessing and ensemble learning for global public health predictions.

🎯 Key Objectives

📊 Perform detailed Exploratory Data Analysis (EDA)

🔍 Implement kNN imputation for missing values

⚡ Benchmark 40+ regression models using LazyPredict

🔧 Apply Hyperparameter Tuning to top-performing models

🤖 Build a highly accurate XGBRegressor model for Life Expectancy prediction

📊 Dataset Overview

Total Records: 2,938

Features: 22

Countries: 193

Years Covered: 15

Target Variable: Life expectancy

Feature Categories
Category	Features
Demographic	Country, Year, Status
Health Factors	Life expectancy, Adult mortality, Infant deaths, Under-five deaths, Hepatitis B, Measles, Polio, Diphtheria, HIV/AIDS, BMI, Thinness indicators
Economic Factors	GDP, Schooling, Income composition of resources, Percentage expenditure, Total expenditure
Population	Population
Categorical	Country (193 unique), Status (Developed/Developing)
🛠️ Methodology and Pipeline
1. Data Preprocessing

🧼 Data cleaning and formatting

🩹 Missing value handling

Mean imputation

kNN Imputation for more accurate estimates

🔠 Categorical Encoding using Label Encoding

2. Model Benchmarking

Used LazyPredict to rapidly train & evaluate 40+ regression models, identifying high-potential candidates.

3. Hyperparameter Tuning

Performed advanced tuning (Grid Search / Random Search + Cross Validation) on the best models to maximize performance.

4. Final Model Selection

Evaluated tuned models on a held-out test set to select the best-performing model.

✅ Results & Conclusion

After extensive tuning, the Optimized XGBRegressor emerged as the best model:

Model	Metric	Score
XGBRegressor (Optimized)	R² Score	96.87%
XGBRegressor (Optimized)	RMSE	Very low

📌 Interpretation:
The optimized model explains almost 97% of the variance in life expectancy — proving strong predictive power and model reliability.

📁 Project Structure
📦 Life-Expectancy-Prediction
├── 📄 README.md
├── 📓 notebooks/
│   └── EDA_and_Model.ipynb
├── 🗂️ data/
│   └── life_expectancy.csv
├── 🧠 models/
│   └── xgb_regressor.pkl
└── 🧪 src/
    ├── preprocessing.py
    ├── model_training.py
    └── evaluation.py

