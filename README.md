# Heart Disease Prediction - Data Science Pipeline

## Overview

This project aims to predict the presence of heart disease in patients using machine learning models. The pipeline includes data ingestion, preprocessing, exploratory data analysis (EDA), feature engineering, model building, evaluation, and optional deployment. The goal is to assist healthcare professionals in early diagnosis and risk assessment.

---

## Dataset

I used the **Cleveland Heart Disease Dataset** from the UCI Machine Learning Repository, also available on [Kaggle](https://www.kaggle.com/datasets/cherngs/heart-disease-cleveland-uci).

### Dataset Features

| Column Name   | Description                                                                 |
|---------------|-----------------------------------------------------------------------------|
| age           | Age in years                                                               |
| sex           | Gender (1 = male, 0 = female)                                               |
| cp            | Chest pain type (0-3)                                                       |
| trestbps      | Resting blood pressure (mm Hg)                                              |
| chol          | Serum cholesterol (mg/dl)                                                   |
| fbs           | Fasting blood sugar > 120 mg/dl (1 = true; 0 = false)                       |
| restecg       | Resting electrocardiographic results (0–2)                                  |
| thalach       | Maximum heart rate achieved                                                 |
| exang         | Exercise-induced angina (1 = yes; 0 = no)                                   |
| oldpeak       | ST depression induced by exercise relative to rest                          |
| slope         | Slope of the peak exercise ST segment                                       |
| ca            | Number of major vessels colored by fluoroscopy (0–3)                        |
| thal          | Thalassemia (3 = normal; 6 = fixed defect; 7 = reversible defect)            |
| target        | Presence of heart disease (0 = no, 1 = yes)                                 |

---

## 🧪 Pipeline Steps

### 1. **Data Collection**
- Load the dataset from local or online repositories.

### 2. **Data Preprocessing**
- Handle missing or invalid values.
- Convert categorical features into numerical format.
- Feature scaling (StandardScaler or MinMaxScaler).
- Split the dataset into training and test sets.

### 3. **Exploratory Data Analysis (EDA)**
- Correlation heatmaps
- Class distribution
- Histograms & boxplots for feature distributions
- Pair plots and target-wise comparisons

### 4. **Feature Engineering**
- Encode categorical variables (`cp`, `thal`, `slope`)
- Create interaction terms (optional)
- Remove low-variance features or highly collinear features

### 5. **Model Building**
- Logistic Regression
- Random Forest
- K-Nearest Neighbors
- XGBoost
- Support Vector Machine (SVM)
- Neural Networks (optional)

### 6. **Model Evaluation**
- Confusion matrix
- ROC-AUC curve
- Accuracy, precision, recall, F1-score
- Cross-validation




Install the required packages using:

```bash
pip install -r requirements.txt
