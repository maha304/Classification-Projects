
# No-show Appointments Prediction

This project builds and evaluates a classification model to predict whether a patient will show up for their scheduled medical appointment. The model is trained using real-world data that includes patient demographics, appointment details, and medical indicators.

---

## 📌 Project Objective

To build a reliable classification model that identifies patients who are likely to miss their appointments, helping healthcare providers take proactive measures to reduce no-shows.

---

## 🔍 Dataset Summary

- Source: Public dataset of medical appointments
- Target variable: `No_show` (1 = No-show, 0 = Showed)
- Key features include:
  - `Days_between` (days between scheduling and appointment)
  - `SMS_received`
  - Appointment weekday
  - Demographics and medical conditions

---

## 🔧 Data Cleaning & Exploratory Analysis

### 1. Data Cleaning
- Removed irrelevant columns such as `PatientId`, `AppointmentID`, `ScheduledDay`, and `AppointmentDay`.
- Converted dates to calculate the `Days_between` feature (i.e., days between scheduling and the appointment).
- Handled missing values and ensured correct data types for all columns.

### 2. Exploratory Data Analysis (EDA)
- Analyzed distributions of key variables like age, gender, and no-show rates.
- Explored correlations between features and the target variable.
- Identified imbalance in the `No_show` variable:
  - Showed: ~79%
  - No-show: ~21%
- Visualized relationships using bar plots and count plots (e.g., no-show rate by weekday or SMS received).

---

## 🛠️ Steps Followed

1. Data cleaning and preprocessing  
2. Handling class imbalance using SMOTE  
3. Feature importance analysis (XGBoost)  
4. Model evaluation with:
   - Random Forest (baseline)
   - XGBoost (final model)
5. Feature selection and re-training  
6. Overfitting and underfitting check  
7. Final model saved as `.pkl`

---

## ✅ Final Model

- Type: **XGBoost Classifier**
- Final features used: 11 selected features
- Balanced data using SMOTE
- Final evaluation shows:

| Metric              | Value  |
|---------------------|--------|
| Accuracy            | 0.717  |
| Precision (No-show) | 0.686  |
| Recall (No-show)    | 0.801  |
| ROC AUC             | 0.788  |

---

## 📁 Files Included

- `final_no_show_model.pkl`: Trained classification model
- `notebook.ipynb`: Full analysis and model building process
- `reduced_features_data.csv`: Cleaned and feature-selected data
- `README.md`: Project summary

---

## 🔄 Future Improvements

- SHAP analysis for model interpretability
- Threshold tuning for better trade-off
- Deployment as a prediction API
