# Financial Failure Prediction

## Problem

Investors, lenders, and analysts need early warning signals that a company may be approaching financial failure. This project tests whether company financial ratios can support reliable failure classification.

## Questions Answered

- Can financial ratios predict whether a company will fail?
- Which approach performs better: Neural Network or Logistic Regression?
- How well do the models identify failed companies?
- What trade-offs appear across accuracy, precision, recall, F1-score, and ROC-AUC?

## Dataset

The panel dataset contains 2,570 company records and financial indicators related to liquidity, profitability, valuation, efficiency, and financial strength. The target is a binary failure classification.

## Model Comparison

| Model | Accuracy | Precision | Recall | F1-score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Neural Network | 0.936 | 0.850 | 0.745 | 0.790 | 0.973 |
| Logistic Regression | 0.927 | 0.805 | 0.728 | 0.760 | 0.962 |

The Neural Network produced the strongest overall results, although Logistic Regression remained competitive and offers greater simplicity and interpretability.

![Financial failure model comparison](../assets/financial-failure-model-comparison.png)

## Repository Contents

- `notebooks/financial-failure-model-comparison.ipynb` — preparation, modeling, and evaluation

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook notebooks/financial-failure-model-comparison.ipynb
```

## Responsible Use

The results are analytical and should not be used as the sole basis for lending or investment decisions. External validation and current financial data are required before operational use.

