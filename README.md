# ❤️ Heart Disease Prediction using Logistic Regression

## 📌 Overview
This project applies a **Logistic Regression model** to predict the presence of heart disease in a patient based on clinical and demographic data. It helps in early detection and preventive healthcare decision-making.

---

## 📂 Data Collection & Description

- **Source**: `data.csv`
- **Features**:
  - `age`
  - `sex`
  - `cp` (chest pain type)
  - `trestbps` (resting blood pressure)
  - `chol` (serum cholesterol)
  - `fbs` (fasting blood sugar)
  - `restecg` (resting electrocardiographic results)
  - `thalach` (maximum heart rate achieved)
  - `exang` (exercise-induced angina)
  - `oldpeak` (ST depression)
  - `slope` (slope of the ST segment)
  - `ca` (number of major vessels)
  - `thal` (thalassemia)
  - `target` (1 = heart disease, 0 = healthy)

**Data Shape**: `(303, 14)`  
**No missing values detected.**

---

## 📊 Data Exploration

- Checked data structure and types.
- Verified absence of missing values.
- Reviewed statistical summary (mean, min, max, etc.).
- Verified distribution of target labels:
  - `1` → Heart Disease (165 cases)
  - `0` → Healthy (138 cases)

---

## 📌 Data Preparation

- **Split data** into:
  - `X` (features)
  - `Y` (target)
- Further split into **Training** and **Test** sets (80:20 ratio) using stratified sampling to maintain label balance.

---

## 📈 Model Training

- **Algorithm Used**: Logistic Regression (sklearn)
- Trained using the training set.
- Encountered convergence warning due to iteration limit; recommended increasing `max_iter` or scaling data for improvement.

---

## 📊 Model Evaluation

- **Training Accuracy**: `85.12%`
- **Test Accuracy**: `81.96%`

---

## 🔮 Predictive System

Built a small prediction system that:
- Takes patient health indicators as input.
- Predicts whether the patient has heart disease (`1`) or not (`0`).

---

## 🚀 Feature Improvements

- **Scale numerical features** to improve model convergence and accuracy.
- **Increase Logistic Regression `max_iter`** to ensure full model convergence.
- **Try alternative classifiers**:
  - Random Forest
  - XGBoost
  - SVM
- **Apply feature selection techniques** (e.g., correlation heatmap, recursive feature elimination) to improve performance.
- **Balance data distribution** if needed with techniques like SMOTE.
- **Hyperparameter tuning** using GridSearchCV for better optimization.
- **Deploy as a web app** using Streamlit or Flask for real-time predictions.

---

