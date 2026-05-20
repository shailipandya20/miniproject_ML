# 🩺 Diabetes Prediction Project

A machine learning project that predicts diabetes using Logistic Regression and Random Forest classifiers on the Pima Indians Diabetes dataset.

---

## 📁 Project Structure

```
diabetes_project/
│
├── diabetes.csv              ← Dataset (download separately)
├── requirements.txt          ← Python dependencies
│
├── main.py                   ← ✅ Run this to execute the full pipeline
├── data_preprocessing.py     ← Load, clean & scale data
├── eda.py                    ← EDA charts (distribution, heatmap)
├── model_training.py         ← Train LR & RF, GridSearchCV tuning
└── visualizations.py         ← Feature importance, comparison, confusion matrix
```

---

## 📥 Dataset

Download `diabetes.csv` from Kaggle:
👉 https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database

Place it in the **same folder** as your Python files.

---

## ⚙️ Setup (One-time)

### 1. Open VS Code and open the project folder
```
File → Open Folder → select diabetes_project/
```

### 2. Create a virtual environment (recommended)
```bash
python -m venv venv
```

### 3. Activate the virtual environment
- **Windows:**
  ```bash
  venv\Scripts\activate
  ```
- **Mac/Linux:**
  ```bash
  source venv/bin/activate
  ```

### 4. Install dependencies
```bash
pip install -r requirements.txt
```

---

## ▶️ How to Run

### Run the full pipeline:
```bash
python main.py
```

### Or run individual modules:
```bash
python data_preprocessing.py   # Test data loading & cleaning
python eda.py                  # Generate EDA charts only
python model_training.py       # Train & evaluate models only
python visualizations.py       # Generate result charts only
```

---

## 📊 Output

Running `main.py` will:
1. Print dataset info and missing values
2. Show & save EDA charts as PNG
3. Train Logistic Regression and Random Forest
4. Run GridSearchCV for hyperparameter tuning
5. Print accuracy and classification reports
6. Save charts:
   - `outcome_distribution.png`
   - `correlation_heatmap.png`
   - `feature_importance.png`
   - `model_comparison.png`
   - `confusion_matrix.png`

---

## 🧠 Models Used

| Model | Description |
|---|---|
| Logistic Regression | Baseline linear classifier |
| Random Forest | Ensemble tree-based classifier |
| Random Forest (Tuned) | GridSearchCV optimized RF |
