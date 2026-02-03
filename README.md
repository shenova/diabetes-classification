# Diabetes Classification from Health Survey Indicators

This repository contains the project for predicting diabetes status using health survey data.

## Problem Overview
We built a **multi-class classification model** to predict diabetes status from survey health indicators:

- **0** – No diabetes (or diabetes only during pregnancy)
- **1** – Prediabetes
- **2** – Diabetes

The dataset is highly imbalanced, making evaluation and model tuning challenging.

## Dataset
This project uses the **Diabetes Health Indicators Dataset** from Kaggle:

🔗 https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset 

**Key details:**
- ~253,680 rows
- 21 health-related features
- Includes demographic and medical indicator variables
 

## Repository Structure
```
.
├── README.md
├── data/
│   └── raw/
├── notebooks/
│   ├── AML_Group_Project_Notebook.ipynb
│   └── AML_Group_Project_Notebook.pdf
└── reports/
    └── AML_Final_Project_Report.pdf
```

## Methods

The following machine learning approaches were explored:

- Multinomial Logistic Regression  
- Logistic Regression with imbalance handling techniques:
  - SMOTE oversampling
  - Random undersampling
  - Class weighting  
- XGBoost with tuned sample weights to improve minority-class performance

## Evaluation

Due to the highly imbalanced class distribution, model performance was evaluated using:

- Accuracy  
- Balanced accuracy  
- Precision, recall, and F1-score for each class  

Special emphasis was placed on improving recall for underrepresented classes, particularly prediabetes.

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/shenova/diabetes-classification.git
cd aml-diabetes-classification
```

2. Make sure you have the required Python libraries installed
(NumPy, pandas, scikit-learn, imbalanced-learn, xgboost, matplotlib, seaborn, and Jupyter).

3. Launch the notebook:
   ```bash
   jupyter notebook
   ```
4. Open the following file:
```bash
diabetes_classification.ipynb
```

