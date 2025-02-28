# Predicting Thyroid Cancer Risk: A Data Science Case Study

## Overview

This project applies machine learning techniques to predict thyroid cancer risk levels (Low, Medium, High) based on clinical, demographic, and lifestyle data collected over a 15-year period. The goal is to identify high-risk patients who may benefit from closer monitoring and to uncover the key factors contributing to thyroid cancer risk.

The project follows the **CRISP-DM framework**, including:

- Data Collection and Understanding
- Data Cleaning and Exploration
- Modeling and Evaluation
- Interpretability and Feature Importance Analysis
- Business Question Review

## Blog Post

For a comprehensive explanation of the project, including visualizations, analysis breakdown, and findings, visit the detailed blog post here:

🔗 [Predicting Thyroid Cancer Risk: A Data Science Case Study](https://medium.com/@cyberspartan228/predicting-thyroid-cancer-risk-a-data-science-case-study-69e1435a9f10)

---

## Repository Structure

```plaintext
|-- data/                       # Folder for dataset
|   |-- thyroid_cancer_risk_data.csv
|-- notebooks/                  # Folder for Jupyter Notebook(s)
|   |-- Thyroid_Cancer_Risk.ipynb
|-- README.md                   # Project Overview
|-- requirements.txt            # Python Environment Requirements
```

---

## Key Findings

- **Top Contributing Factors**: Nodule Size, TSH Level, Radiation Exposure
- **Model Performance**: Best model (Tuned Random Forest) achieved 66.86% accuracy.
- **Interpretability**: SHAP analysis highlighted clinical factors as primary risk indicators.
- **Lifestyle Factors**: Smoking and obesity contributed minimally compared to clinical data.

---

## Detailed Model Evaluation & Metrics Justification

### Final Model Selected

- **Model**: Random Forest Classifier (Tuned)
- **Final Accuracy**: 66.86%

### Final Model Parameters

| Parameter               | Value |
| ----------------------- | ----- |
| **n\_estimators**       | 200   |
| **max\_depth**          | 20    |
| **min\_samples\_split** | 5     |

### Explanation

- **n\_estimators**: Increased to 200 to improve generalization by averaging across more trees.
- **max\_depth**: Capped at 20 to avoid overfitting while maintaining flexibility.
- **min\_samples\_split**: Increased to 5 to prevent small, noisy splits.

### Class-Level Performance (Random Forest)

| Risk Level      | Precision | Recall | F1-Score |
| --------------- | --------- | ------ | -------- |
| Low Risk (0)    | 1.00      | 1.00   | 1.00     |
| Medium Risk (1) | 0.50      | 0.53   | 0.52     |
| High Risk (2)   | 0.51      | 0.48   | 0.49     |

### Metrics Justification

- **Accuracy**: Overall correctness across all patients.
- **Precision**: Important for high-risk patients to ensure flagged patients truly require attention.
- **Recall**: Crucial for identifying all at-risk patients to avoid missed diagnoses.
- **F1-Score**: Balances precision and recall, especially useful for **Medium** and **High** risk.
- **Class-Level Reporting**: Essential to highlight strengths and weaknesses in each risk category, exposing issues hidden by overall accuracy.

These metrics were chosen to ensure a balanced evaluation that considers:

- **The critical need to correctly identify high-risk patients.**
- **The asymmetric costs of false positives vs. false negatives in a healthcare context.**
- **The importance of handling class imbalance.**

---

## Instructions to Reproduce

1. Clone the repository.
2. Install dependencies using `pip install -r requirements.txt`.
3. Run `notebooks/Thyroid_Cancer_Risk.ipynb` for full analysis.

---

## Requirements

All required packages are listed in `requirements.txt`.

---

## References

- SHAP Documentation: [https://shap.readthedocs.io/](https://shap.readthedocs.io/)
- Scikit-learn Documentation: [https://scikit-learn.org/](https://scikit-learn.org/)
- CRISP-DM Process: [https://www.datascience-pm.com/crisp-dm-2/](https://www.datascience-pm.com/crisp-dm-2/)

---

## Contact

Author: CyberSpartan228

For further inquiries, visit the blog post: [Medium Post](https://medium.com/@cyberspartan228/predicting-thyroid-cancer-risk-a-data-science-case-study-69e1435a9f10)


For further inquiries, visit the blog post: Medium Post



