# 🏦 Loan Approval Prediction

## 📌 Project Overview
This project is part of my **Elevvo Machine Learning Internship (Task 4)**.  
The goal is to **predict loan approval status** using machine learning techniques while handling **imbalanced data**.  

The project compares **Logistic Regression** and **Decision Tree Classifier**, with and without **SMOTE oversampling**.

---

## 📂 Repository Structure
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

## ⚙️ Workflow
1. **Data Preprocessing**
   - Handled missing values (mode/median imputation).
   - Encoded categorical variables using one-hot encoding.
   - Scaled numerical features with `StandardScaler`.

2. **Exploratory Data Analysis (EDA)**
   - Visualized loan approval status distribution.
   - Plotted categorical distributions.

3. **Model Training**
   - Logistic Regression (baseline model).
   - Decision Tree Classifier.
   - Both trained **before and after SMOTE** to handle imbalance.

4. **Evaluation Metrics**
   - Accuracy
   - Precision
   - Recall
   - F1 Score
   - Confusion Matrices

---

## 📊 Results

### 🔹 Logistic Regression (No SMOTE)
- **Accuracy:** 0.8618  
- **Precision:** 0.84  
- **Recall:** 0.9882  
- **F1 Score:** 0.9081  

### 🔹 Decision Tree (No SMOTE)
- **Accuracy:** 0.7479  
- **Precision:** 0.8214  
- **Recall:** 0.8117  
- **F1 Score:** 0.8166  

---

### 🔹 Logistic Regression (With SMOTE)
- **Accuracy:** 0.8374  
- **Precision:** 0.8350  
- **Recall:** 0.9529  
- **F1 Score:** 0.8901  

### 🔹 Decision Tree (With SMOTE)
- **Accuracy:** 0.7398  
- **Precision:** 0.8441  
- **Recall:** 0.7647  
- **F1 Score:** 0.8025  

---

## ✅ Key Insights
- Logistic Regression consistently outperformed Decision Tree.  
- SMOTE improved **recall** for both models but slightly reduced overall accuracy.  
- Logistic Regression + SMOTE achieved the **best balance** (Recall: 0.95, F1: 0.89).  

---

## 🛠️ Tools & Libraries
- Python  
- Pandas | NumPy  
- Matplotlib | Seaborn  
- Scikit-learn  
- imbalanced-learn (SMOTE)  

---

## 📌 How to Run
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

## 📸 Visuals
Some key plots are saved in the `visuals/` folder:

- Loan status distribution  
- Confusion matrices (LogReg & Decision Tree, with/without SMOTE)  
- Model comparison bar charts  

---

## 👤 Author
**AlaEldin Ali**  

_Data Science Enthusiast | ML Intern @ Elevvo_  

🔗 [LinkedIn](https://www.linkedin.com/in/x3loox) | [GitHub](https://github.com/x3loox)

---

## 📜 License
This project is for **educational purposes** as part of the Elevvo Pathways internship.
