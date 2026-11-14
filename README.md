# An Explainable Hybrid Machine Learning Approach for Phishing Website Detection

A machine learning project that detects phishing websites using hybrid models and explains the predictions with SHAP. Built in Python on Google Colab.

## What it does

- Classifies a website as phishing or legitimate
- Compares Logistic Regression, Random Forest, and XGBoost
- Builds two hybrid models: a soft-voting ensemble and a stacking ensemble
- Explains predictions with SHAP, showing which features push a website toward phishing

## Datasets

- **PhiUSIIL Phishing URL dataset:** 235,795 websites, used for data exploration, feature importance, and testing how the model behaves when top features are removed
- **UCI Phishing Websites dataset:** 11,055 websites with 30 features, used to train and compare the hybrid models

## Results (UCI dataset)

| Model | Accuracy | ROC AUC |
|-------|----------|---------|
| Random Forest | 97.5% | 0.9964 |
| XGBoost | 96.2% | 0.9944 |
| Voting Hybrid | 96.5% | 0.9954 |
| Stacking Hybrid | 97.6% | 0.9973 |

On the PhiUSIIL dataset, Random Forest reached about 99.98% accuracy even after removing the most influential features, which shows many features carry strong signal.

## Tech used

- Python, pandas, NumPy
- scikit-learn, XGBoost
- SHAP
- Matplotlib
- Google Colab

## Course

CSE 437, BRAC University
