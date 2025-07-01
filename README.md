# 🩺 Cardiovascular Disease Prediction with Logistic Regression

This project applies **logistic regression** to a real-world cardiovascular disease dataset. The main objective is to interpret the relationship between health indicators and cardiovascular disease using **odds ratios**, alongside building a predictive model.

## 📊 Dataset

- **Source**: [Cardiovascular Disease Dataset on Kaggle](https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset)
- **Records**: 69,000+ patient entries
- **Target**: Binary label indicating presence or absence of cardiovascular disease

## 🧾 Feature Descriptions

| Column         | Description                                      |
|----------------|--------------------------------------------------|
| `age`          | Age in days                                      |
| `gender`       | 1 = women, 2 = men                               |
| `height`       | Height in cm                                     |
| `weight`       | Weight in kg                                     |
| `ap_hi`        | Systolic blood pressure                          |
| `ap_lo`        | Diastolic blood pressure                         |
| `cholesterol`  | 1 = normal, 2 = above normal, 3 = well above normal |
| `gluc`         | 1 = normal, 2 = above normal, 3 = well above normal |
| `smoke`        | Binary: 1 = smoker, 0 = non-smoker               |
| `alco`         | Binary: 1 = drinks alcohol, 0 = does not         |
| `active`       | Binary: 1 = physically active, 0 = not           |
| `cardio`       | Target: 1 = has disease, 0 = healthy             |


## 🚀 What the Project Does

- Preprocesses real health data
- Trains a logistic regression model with `GridSearchCV` for optimal hyperparameters
- Saves the final model and scaler using `joblib`
- Trains a second **unregularized**, **unscaled** model to calculate **odds ratios**
- Demonstrates interpretability using real-world health features


## 🔍 Key Insight from Odds Ratios

- **Cholesterol (ordinal)**  
  → A one-level increase in cholesterol (normal → above normal → well above normal) increases odds of cardiovascular disease by **50%**  
  *(Odds Ratio = 1.5)*


## 💡 Technologies Used

- Python
- pandas, NumPy
- scikit-learn
- joblib

