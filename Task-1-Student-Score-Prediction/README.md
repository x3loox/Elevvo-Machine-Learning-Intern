
# 🎯 Student Score Prediction

This project is part of the **Elevvo Machine Learning Internship** (Task 1: Level 1).  
The goal is to **predict students' exam scores** based on factors like study hours, sleep, attendance, and motivation using **linear and polynomial regression** models.

---

## 📁 Dataset

- Source: [Student Performance Factors](https://www.kaggle.com/datasets/lainguyn123/student-performance-factors?phase=FinishSSORegistration&returnUrl=%2Fdatasets%2Flainguyn123%2Fstudent-performance-factors%2Fversions%2F8%3Fresource%3Ddownload&SSORegistrationToken=CfDJ8H3GHv39YMxDjEpKbXZX9wGG9mUqQlT1KP2VAwid2FLZmTVOSU6TEmYKZQ6s3zWXvOgVQ-szXKDVfwh086NIxBGKTtOOwl0kdaiNxO4peH4OjJnfUs1hpalbujn0-6DYPfsJ58XR1tN9CxL8sI772cIOZrX_uaD3s93ZFkeMjUDWQUC4aaLVLfHQW-_L4WbktlfmqJoQNqbHsUbKtUcTY8aMB7msiG5p8CKuA079b2X3up0f_XludR70LVOk60C_SHLwuCkXKtn95CBONkMJpJnoMzDH48xqkMxnb3OGofbO96oShxiWw_Qn4cxKwaMNeTVxngzHeTUp0-G_kU9ECaf2raQ&DisplayName=Alex) (Kaggle)
- Format: CSV (`StudentPerformanceFactors.csv`)
- Target Variable: `Exam_Score`

---

## 🔧 Tools & Libraries

- Python 🐍
- pandas
- matplotlib
- seaborn
- scikit-learn

---

## 🧪 Project Steps

1. **Data Cleaning**
   - Handled missing values
2. **Data Visualization**
   - Scatter plots and regression lines
   - Correlation analysis
3. **Linear Regression**
   - Train-test split (80/20)
   - Evaluated with MAE, MSE, R²
4. **Polynomial Regression**
   - Degree = 2
   - Compared performance with linear regression
5. **Feature Engineering**
   - Introduced `Motivation_Level_Num` (encoded from categorical)
   - Trained a new regression model using additional features:
     - `Previous_Scores`, `Sleep_Hours`, `Attendance`, etc.

---

## 📊 Evaluation Metrics

- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **R² Score**

---

## 📈 Results Summary

| Model                 | R² Score (Test) | MAE       | MSE       |
|----------------------|----------------|-----------|-----------|
| Linear Regression     | ~0.21          | ~2.5      | ~12.3      |
| Polynomial Regression | ~0.21+         | ~2.5      | ~12.5      |
| Extended Features     | ~0.60+         | ~1.4      | ~6.5      |

> 🚀 Adding features like `Sleep_Hours`, `Attendance`, and `Motivation` significantly improved performance.

---

## ▶️ How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/x3loox/Elevvo-Machine-Learning-Intern/blob/main/Task-1-Student_Score_Prediction.git
   cd Task-2-Customer-Segmentation
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook Student_Score_Prediction.ipynb
   ```

---

## 🧠 Bonus Ideas

- Use more advanced models (e.g., Random Forest)
- Hyperparameter tuning
- Cross-validation
- Add feature importance visualization

---

## 🤝 Internship Task Info

- **Internship**: Elevvo – Machine Learning Track
- **Task Level**: Level 1 – Task 1
- **Duration**: 1 Month (Minimum 4 tasks required)

---

## 👤 Author
**AlaEldin Ali**  

_Data Science Enthusiast | ML Intern @ Elevvo_  

🔗 [LinkedIn](https://www.linkedin.com/in/x3loox) | [GitHub](https://github.com/x3loox)

---

## 📜 License
This project is for **educational purposes** as part of the Elevvo Pathways internship.
