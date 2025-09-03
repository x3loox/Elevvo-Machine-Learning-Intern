# 🌲 Forest Cover Type Classification

## 📌 Project Overview
This project is part of my **Elevvo Pathways Machine Learning Internship (Task 3)**.  
The objective is to classify the type of forest cover based on cartographic and environmental features using **multi-class classification** techniques.

Dataset used: [Covertype (UCI Repository)](https://archive.ics.uci.edu/ml/datasets/covertype)

---

## 🎯 Objectives
- Load, clean, and preprocess the dataset.
- Handle categorical and numerical features appropriately.
- Train and evaluate **Random Forest** and **XGBoost** classifiers.
- Compare model performance with accuracy, confusion matrices, and feature importance.
- Apply **hyperparameter tuning** to optimize both models.

---

## 🛠️ Tools & Libraries
- **Python**
- **Pandas** – Data manipulation
- **Matplotlib & Seaborn** – Visualization
- **Scikit-learn** – Random Forest, preprocessing, evaluation
- **XGBoost** – Gradient boosting classifier

---

## 🌲 Dataset

This project uses the Forest CoverType dataset from the UCI ML Repository.

- 🔗 [Download Full Dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/covtype/covtype.data.gz)
- 📄 A sample (`data/sample_covtype.csv`) is included for quick testing.


---

## 📊 Steps Followed
1. **Load Dataset**
   - UCI Covertype dataset with 581,012 samples and 54 features.
   - Target variable: `Cover_Type` (7 forest cover classes).

2. **Data Exploration**
   - Checked for missing values (none found).
   - Visualized target distribution.
   - Correlation heatmap for numeric features.

3. **Model Training**
   - **Random Forest Classifier** (baseline model).
   - **XGBoost Classifier** (gradient boosting approach).

4. **Model Evaluation**
   - Accuracy scores.
   - Confusion Matrices.
   - Feature Importance analysis.

5. **Hyperparameter Tuning**
   - GridSearchCV for Random Forest.
   - RandomizedSearchCV for XGBoost.

---

## 📈 Results

### ✅ Accuracy (Before Tuning)
- **Random Forest:** 0.9533  
- **XGBoost:** 0.8696  

### ⚡ Best Hyperparameters Found
- **Random Forest:**  
  ```python
  {'max_depth': None, 'min_samples_leaf': 1, 'min_samples_split': 2, 'n_estimators': 200}
  ```
  Best RF Score (Train CV): **0.9468**

- **XGBoost:**  
  ```python
  {'subsample': 1.0, 'n_estimators': 200, 'max_depth': 10, 'learning_rate': 0.2, 'gamma': 0, 'colsample_bytree': 1.0}
  ```
  Best XGB Score (Train CV): **0.9538**

### 📊 Final Comparison
| Model            | Accuracy (Before Tuning) | Accuracy (After Tuning) |
|------------------|--------------------------|--------------------------|
| Random Forest    | 0.9533                   | 0.9468 (CV Score)        |
| XGBoost          | 0.8696                   | 0.9538 (CV Score)        |

---

## 🔍 Key Insights
- **Random Forest** performed better out-of-the-box with very high accuracy.  
- **XGBoost** initially underperformed but achieved competitive performance after hyperparameter tuning.  
- Feature importance analysis highlighted **Elevation, Horizontal Distance to Roadways, and Hillshade features** as strong predictors.  

---

## 📂 Project Structure
```
forest-cover-classification/
│── data/
│   └── sample_covtype.csv
│── visuals/
│   ├── confusion_matrix_rf.png
│   ├── confusion_matrix_xgb.png
│   ├── corr_heatmap.png
│   ├── distribution_cover_types.png
│   ├── feature_importance_rf.png
│   ├── feature_importance_xgb.png
│   ├── model_comparison.png
│── forest_cover_classification.ipynb
│── README.md
│── requirements.txt
```

---

## 🚀 Next Steps
- Try **LightGBM** or **CatBoost** for further comparison.
- Perform feature engineering to reduce dimensionality.
- Deploy the best model using **Streamlit** for interactive predictions.

---

## 🏷️ Tags
#DataScience #MachineLearning #Classification #RandomForest #XGBoost #ElevvoPathways #Internship #Python

---

## 📜 License
This project is for **educational purposes** as part of the Elevvo Pathways internship.
