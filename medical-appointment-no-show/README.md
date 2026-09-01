# Medical Appointment No-show Prediction

## Problem

Missed medical appointments waste clinical capacity, increase waiting times, and delay patient care. This project identifies appointments at higher risk of a no-show so healthcare teams can target reminders and interventions.

## Questions Answered

- Which patients are most likely to miss an appointment?
- How do waiting time, age, SMS reminders, appointment day, and medical conditions relate to attendance?
- How should the imbalance between attended and missed appointments be handled?
- Which model provides the strongest recall for no-show patients?

## Approach

1. Clean appointment and demographic data.
2. Engineer features such as the time between scheduling and appointment.
3. Explore attendance patterns and target imbalance.
4. Balance training data using SMOTE.
5. Compare baseline Random Forest and XGBoost classifiers.
6. Select the most useful features and evaluate the final model.

## Final Results

| Metric | Score |
|---|---:|
| Accuracy | 0.717 |
| Precision — No-show | 0.686 |
| Recall — No-show | 0.801 |
| ROC AUC | 0.788 |

The final XGBoost workflow uses 11 selected features. Its 80.1% no-show recall is particularly relevant when the priority is identifying as many at-risk appointments as possible.

![Appointment attendance by medical factors](../assets/no-show-medical-factors.png)

## Repository Contents

- `data/` — raw and cleaned appointment data
- `notebooks/01-exploratory-analysis.ipynb` — cleaning and EDA
- `notebooks/02-modeling.ipynb` — modeling and evaluation
- `outputs/no_show_eda_summary.pdf` — EDA summary report

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook
```

Run the analysis notebook before the prediction notebook.

## Future Improvements

SHAP interpretation, decision-threshold tuning, validation on newer data, and deployment as a prediction API.

