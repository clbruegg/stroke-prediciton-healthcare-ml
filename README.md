# Stroke Prediction Using Healthcare Data  
**Machine Learning Classification Project**

![License](https://img.shields.io/badge/License-MIT-green)
![Python](https://img.shields.io/badge/Python-3.8+-blue)

**Authors:** Collin Brueggeman  
**Dataset:** Kaggle Stroke Prediction Dataset (5,110 records)

[**Full Project Report (PDF)**](./reports/Brueggeman_Stroke_Prediction.pdf)  
[**Presentation Slides (PPTX)**](./presentation/)  
[**Reproducible Notebooks**](./notebooks/)

---

## Project Overview
- **Problem**: Predict stroke risk from patient health records (binary classification)
- **Key Techniques**: Median imputation (BMI), outlier capping, binary/one-hot encoding, StandardScaler, **SMOTE** for severe class imbalance (only 4.87% stroke cases)
- **Models Tested**: Logistic Regression, SVM, Decision Tree
- **Best Model**: **Decision Tree** — 91.4% accuracy, 91.5% F1-score after GridSearchCV tuning

---

## Key Results (Tuned Models)

| Model              | Accuracy | Precision | Recall | F1-Score |
|--------------------|----------|-----------|--------|----------|
| Logistic Regression| 0.857    | 0.833     | 0.891  | 0.861    |
| SVM                | 0.887    | 0.859     | 0.927  | 0.891    |
| **Decision Tree**  | **0.914**| **0.908** | **0.922**| **0.915**|

- Top predictors: Age, hypertension, heart disease, avg_glucose_level, BMI  
- ROC curves and confusion matrices in the notebook

---

## Repository Structure
- `data/` — Raw + cleaned CSV files  
- `notebooks/` — Full EDA, preprocessing, modeling, and evaluation  
- `reports/` — Detailed PDF report  
- `presentation/` — Slides for demo/presentation

---

## How to Run
1. Open `notebooks/`  
2. Run cells sequentially (data is included)

---

## Technologies & Topics
`machine-learning` `stroke-prediction` `classification` `healthcare` `smote` `decision-tree` `jupyter-notebook` `imbalanced-data`

---

## How to Cite

```bibtex
@misc{brueggeman2025stroke,
  author       = {Brueggeman, Collin},
  title        = {Stroke Prediction Using Healthcare Data},
  year         = {2025},
  howpublished = {GitHub},
  url          = {https://github.com/Brueggs/stroke-prediction-healthcare-ml}
}
