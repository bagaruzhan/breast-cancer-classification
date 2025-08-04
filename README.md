# Breast Cancer Classification — ML Model Comparison

This project performs a full machine learning pipeline to classify breast cancer using clinical features. It compares 7 classification algorithms and explains the best model using SHAP.

## Objectives
- Explore and understand the dataset (EDA)
- Train and compare 7 classification models
- Optimize the best model (Logistic Regression)
- Interpret predictions using SHAP

## Dataset
- Source: [Kaggle](https://www.kaggle.com/datasets/wasiqaliyasir/breast-cancer-dataset/data)
- 569 samples, 30 numerical features
- Target: `diagnosis` (`M` = 0, `B` = 1)

## Models Compared
- Logistic Regression 
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Naive Bayes
- Decision Tree
- Random Forest
- XGBoost

## Final Results
| Metric     | Score    |
|------------|----------|
| Accuracy   | 98.6%    |
| Precision  | 98.9%    |
| Recall     | 98.9%    |
| F1-score   | 98.9%    |

## Model Explainability (SHAP)
Top influential features:
- `radius_worst`
- `texture_worst`
- `area_worst`

## How to Run
```bash
git clone https://github.com/bagaruzhan/breast-cancer-classification.git
cd breast-cancer-classification
pip install -r requirements.txt
jupyter notebook breast_cancer_ml.ipynb
