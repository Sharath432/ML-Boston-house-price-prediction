🏠 Boston Housing Price Prediction
This project predicts housing prices in Boston using various features such as number of rooms, crime rate, and distance to employment centers. It uses data preprocessing, exploratory data analysis, feature engineering, and machine learning with hyperparameter tuning to build an accurate predictive model.

📁 Dataset
Source: Boston Housing Dataset (CSV file)

Target Variable: MEDV – Median value of owner-occupied homes in $1000s

Features:

CRIM, ZN, INDUS, CHAS, NOX, RM, AGE, DIS, RAD, TAX, PTRATIO, B, LSTAT

Engineered: LOG_CRIM, LOG_LSTAT

🔍 Problem Statement
To predict the median house price (MEDV) for different areas in Boston based on socio-economic and geographic data using machine learning regression models.

🛠️ Tasks Performed
Data Cleaning

Renamed columns, handled missing/duplicate values, converted categorical types

Exploratory Data Analysis (EDA)

Visualized distributions, correlations, boxplots to understand relationships

Feature Engineering

Log transformation on skewed features (CRIM, LSTAT)

Feature scaling using StandardScaler

Model Building & Evaluation

Split data into train/test sets (80/20)

Applied multiple regression models

Performed GridSearchCV to tune RandomForestRegressor

Model Evaluation Metrics

Root Mean Squared Error (RMSE)

R² Score

✅ Best Model: Random Forest Regressor
Best Parameters: (from GridSearchCV)

n_estimators: 150

max_depth: 5

min_samples_split: 4

Evaluation:

R² Score: e.g., 0.87

RMSE: e.g., 3.21

📈 Tools & Libraries Used
pandas, numpy for data handling

seaborn, matplotlib for visualization

scikit-learn for ML models, scaling, cross-validation

📌 How to Run
bash
Copy
Edit
1. Clone this repo
2. Make sure required libraries are installed
3. Run the Python notebook or script
📦 Future Improvements
Save and deploy the model using joblib or pickle

Build a Streamlit dashboard for live predictions

Test on real-world unseen housing data
