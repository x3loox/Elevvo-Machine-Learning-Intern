# Loan Approval Prediction
**Machine Learning Case Study | Elevvo ML Internship**

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue?style=plastic&logo=python)](https://www.python.org/)
[![Scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange?style=plastic&logo=scikitlearn)](https://scikit-learn.org/)
[![Status](https://img.shields.io/badge/Status-Completed-success?style=plastic)](#)
[![Internship](https://img.shields.io/badge/Experience-ML%20Intern-blueviolet?style=plastic)](#)

---

## Table of Contents
1. [Business Context](#business-context--problem-statement)
2. [Repository Structure](#repository-structure)
3. [Dataset Overview](#dataset-overview)
4. [Methodology](#methodology--workflow)
5. [Evaluation Metrics](#evaluation-metrics)
6. [Results](#results-summary)
7. [Key Insights](#key-insights--business-interpretation)
8. [Model Selection](#model-selection-rationale)
9. [Limitations](#limitations--future-improvements)
10. [Tools & Technologies](#tools--technologies)
11. [How to Run](#how-to-run-the-project)
12. [Author](#author)
13. [License](#license) 

---

## Business Context & Problem Statement

Financial institutions face a critical trade-off when approving loans:

- ❌ Approving high-risk applicants leads to financial loss  
- ❌ Rejecting eligible applicants results in lost revenue and reduced customer trust  

The objective of this project is to build a **machine learning model that predicts loan approval decisions**, with a strong focus on **handling imbalanced data** and **minimizing false negatives**.

This project was completed as part of my **Machine Learning Internship at Elevvo**, following an end-to-end data science workflow.

---

## Repository Structure
```
Task-4-Loan-Approval-Prediction/
│── data/
│   └── loan_data.csv
│── notebooks/
│   └── loan_approval_prediction.ipynb
│── visuals/
│   ├── loan_status_distribution.png
│   ├── confusion_matrix_logreg_no_smote.png
│   ├── confusion_matrix_logreg_with_smote.png
│   ├── confusion_matrix_dcitree_no_smote.png
│   ├── confusion_matrix_dcitree_with_smote.png
│   ├── modeles_comparison.png
│── README.md
```
---

## Dataset Overview

- **Type:** Tabular structured data  
- **Target variable:** Loan approval status  
- **Key challenge:** Class imbalance  
- **Features include:** Applicant demographics, financial indicators, and loan attributes

---

## Methodology & Workflow

### Data Preprocessing
- Missing values handled using **median and mode imputation**
- Categorical variables encoded using **one-hot encoding**
- Numerical features scaled with **StandardScaler**

### Exploratory Data Analysis (EDA)
- Loan approval distribution analysis
- Categorical feature visualization
- Detection of imbalance patterns

### Model Training
- Logistic Regression (baseline & interpretable)
- Decision Tree Classifier
- Models trained **with and without SMOTE**

---

## Evaluation Metrics

- Accuracy  
- Precision  
- Recall  
- F1 Score  
- Confusion Matrix  

> **Recall was prioritized** due to its business importance in reducing rejected eligible applicants.

---

## Results Summary

### Logistic Regression (No SMOTE)
- Accuracy: **0.86**
- Precision: **0.84**
- Recall: **0.99**
- F1 Score: **0.91**

### Decision Tree (No SMOTE)
- Accuracy: **0.75**
- Precision: **0.82**
- Recall: **0.81**
- F1 Score: **0.82**

### Logistic Regression (With SMOTE)
- Accuracy: **0.84**
- Precision: **0.84**
- Recall: **0.95**
- F1 Score: **0.89**

### Decision Tree (With SMOTE)
- Accuracy: **0.74**
- Precision: **0.84**
- Recall: **0.76**
- F1 Score: **0.80**

---

## Key Insights & Business Interpretation

- Logistic Regression consistently outperformed Decision Trees
- SMOTE improved recall while slightly reducing accuracy
- Logistic Regression + SMOTE achieved the best business trade-off
- Higher recall reduces missed revenue opportunities

---

## Model Selection Rationale

Logistic Regression was selected due to:
- Interpretability for financial decision-making
- Stability on imbalanced datasets
- Lower overfitting risk
- Easier regulatory explanation

---

## Limitations & Future Improvements

- Dataset size is limited
- Advanced models (XGBoost, LightGBM) could be explored
- Threshold optimization could improve decision boundaries
- Deployment and monitoring were not included

---

## Tools & Technologies

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- imbalanced-learn (SMOTE)

---

## How to Run the Project
1. Clone this repository:
   ```bash
   git clone https://github.com/x3loox/Elevvo-Machine-Learning-Intern/tree/main/Task-4-Loan-Approval-Prediction.git
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Open the notebook:
   ```bash
   jupyter notebook notebooks/loan_approval_prediction.ipynb
   ```

---

## Author
**AlaEldin Ali**  

_Data Science Enthusiast | Machine Learning Intern @ Elevvo_  

🔗 [LinkedIn](https://www.linkedin.com/in/x3loox) | [GitHub](https://github.com/x3loox)

---

## License
This project was developed for **educational purposes** as part of the **Elevvo Pathways Machine Learning Internship**.
