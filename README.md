# 🩺 Diabetes Prediction Project
A machine learning project that predicts diabetes using Logistic Regression and Random Forest classifiers on the Pima Indians Diabetes dataset.

## Project Structure
```
diabetes_project/
│
├── diabetes.csv              ← Dataset (download separately)
├── requirements.txt          ← Python dependencies
│
├── main.py                   ← Run this to execute the full pipeline
├── data_preprocessing.py     ← Load, clean & scale data
├── eda.py                    ← EDA charts (distribution, heatmap)
├── model_training.py         ← Train LR & RF, GridSearchCV tuning
└── visualizations.py         ← Feature importance, comparison, confusion matrix
```
## Dataset

Download `diabetes.csv` from Kaggle:
👉 https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database

## Models Used

1. Logistic Regression -> Baseline linear classifier
2. Random Forest -> Ensemble tree-based classifier
3. Random Forest (Tuned) -> GridSearchCV optimized RF

## 📊 Output

Running `main.py` will:
1. Print dataset info and missing values
2. Show & save EDA charts as PNG
3. Train Logistic Regression and Random Forest
4. Run GridSearchCV for hyperparameter tuning
5. Print accuracy and classification reports



