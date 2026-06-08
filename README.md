# Temperature Prediction Using Machine Learning

## Overview

This project aims to predict temperature using weather and geographical data such as humidity, pressure, latitude, and longitude. Multiple machine learning algorithms were implemented and compared to determine the most accurate model for temperature prediction.

The project follows a complete machine learning pipeline including data preprocessing, feature engineering, model training, evaluation, and model comparison.

---

## Objective

To build an accurate machine learning model that predicts temperature based on environmental and geographical conditions.

---

## Dataset

The dataset contains over 700,000 weather observations with the following features:

| Feature | Description |
|----------|------------|
| humidity | Relative humidity (%) |
| pressure | Atmospheric pressure |
| lat | Latitude |
| lon | Longitude |
| temperature | Target variable |

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- XGBoost
- Jupyter Notebook

---

## Project Workflow

### 1. Data Collection
- Loaded the weather dataset using Pandas.

### 2. Data Cleaning
- Removed duplicate records.
- Handled missing values.
- Removed unnecessary columns.
- Ensured no data leakage during feature engineering.

### 3. Exploratory Data Analysis (EDA)
- Summary statistics
- Correlation analysis
- Distribution plots
- Feature relationship analysis

### 4. Feature Engineering
Created additional features:

- Humidity × Pressure
- Humidity²
- Pressure²

### 5. Data Preprocessing
- Train-Test Split (80:20)
- Feature Scaling for Linear and Polynomial Regression models

### 6. Model Building

Implemented and compared:

- Linear Regression
- Polynomial Regression
- Random Forest Regressor
- XGBoost Regressor

### 7. Model Evaluation

Models were evaluated using:

- R² Score
- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)

---

## Model Performance

| Model | R² Score | RMSE | MAE |
|---------|---------:|---------:|---------:|
| XGBoost | 0.9009 | 2.0335 | 1.4665 |
| Random Forest | 0.8866 | 2.1750 | 1.5906 |
| Polynomial Regression | 0.8175 | 2.7588 | 2.0572 |
| Linear Regression | 0.6528 | 3.8054 | 2.6855 |

---

## Best Model

### XGBoost Regressor

Performance Metrics:

- R² Score: 0.9009
- RMSE: 2.0335
- MAE: 1.4665

XGBoost achieved the highest predictive performance, explaining approximately 90% of the variance in temperature values while maintaining low prediction error.

---

## Project Structure

text Temperature-Prediction/ │ ├── humidity.csv ├── temp_pred.ipynb ├── README.md └── requirements.txt 

---

## Installation & Usage

### Clone the Repository

bash git clone https://github.com/Rishabh-Tiwari-18/Temperature-Prediction.git 

### Install Required Libraries

bash pip install -r requirements.txt 

### Run the Project

bash jupyter notebook 

Open:

text temp_pred.ipynb 

---

## Key Learnings

- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Regression Modeling
- Ensemble Learning
- Model Evaluation & Comparison
- Machine Learning Workflow

---

## Future Improvements

- Hyperparameter Optimization
- Cross Validation
- Feature Selection Techniques
- Time-Series Forecasting Models
- Deep Learning Approaches

---
