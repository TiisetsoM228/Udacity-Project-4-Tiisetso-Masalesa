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

## Instructions to Reproduce
1. Clone the repository.
2. Install dependencies using `pip install -r requirements.txt`.
3. Run `notebooks/Thyroid_Cancer_Risk.ipynb` for full analysis.

---

## Requirements
All required packages are listed in `requirements.txt`.

---

## References
- SHAP Documentation: https://shap.readthedocs.io/
- Scikit-learn Documentation: https://scikit-learn.org/
- CRISP-DM Process: https://www.datascience-pm.com/crisp-dm-2/

---

## Contact
Author: CyberSpartan228

For further inquiries, visit the blog post: [Medium Post](https://medium.com/@cyberspartan228/predicting-thyroid-cancer-risk-a-data-science-case-study-69e1435a9f10)

