# Customer Segmentation using Clustering

## 📌 Project Overview
This project is part of my **Elevvo Pathways Internship** (Task 2).  
The goal is to cluster **mall customers** into different segments based on their **Annual Income** and **Spending Score** using **unsupervised learning techniques**.  
We also experiment with alternative clustering algorithms like **DBSCAN**.

---

## 🎯 Objectives
- Perform **data exploration** and **visualization**.
- Scale features using **MinMaxScaler**.
- Apply **K-Means Clustering** and find the optimal number of clusters using the **Elbow Method**.
- Visualize customer segments in 2D.
- Bonus: Apply **DBSCAN** clustering for comparison.
- Analyze **average spending score per cluster**.

---

## 📂 Dataset
- **Source**: [Mall Customers Dataset (Kaggle)](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial)
- **File**: `Mall_Customers.csv`
- **Features**:
  - `CustomerID`
  - `Gender`
  - `Age`
  - `Annual Income (k$)`
  - `Spending Score (1-100)`

---

## 🛠️ Tools & Libraries
- **Python**
- **Pandas** – Data manipulation
- **NumPy** – Numerical computing
- **Matplotlib** & **Seaborn** – Data visualization
- **Scikit-learn** – Machine learning algorithms & preprocessing

---

## 📊 Steps Followed
1. **Load and Explore Data**  
   - Check for missing values  
   - View basic statistics
2. **Initial Visualization**  
   - Scatter plot of Income vs Spending Score
3. **Data Scaling**  
   - Normalize data using MinMaxScaler
4. **K-Means Clustering**  
   - Find optimal `k` with the Elbow Method  
   - Train model and visualize clusters
5. **DBSCAN Clustering (Bonus)**  
   - Determine `eps` using K-Distance plot  
   - Train DBSCAN and compare clusters
6. **Cluster Analysis**  
   - Calculate mean spending score per cluster  
   - Bar plots for cluster spending patterns

---

## 📷 Visuals
- **Elbow Method Plot** – Determine optimal number of clusters
- **K-Means Clusters** – Customer segmentation visualization
- **DBSCAN Clusters** – Alternative clustering method
- **Average Spending Score per Cluster** – Cluster-level spending behavior

---

## ▶️ How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/x3loox/Elevvo-Machine-Learning-Intern/blob/main/Task-2-Customer-Segmentation.git
   cd Task-2-Customer-Segmentation
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook notebooks/customer_segmentation.ipynb
   ```

---

## 📌 Learning Outcomes
- Understanding **unsupervised learning** concepts.
- Applying **K-Means** and **DBSCAN** clustering in real datasets.
- Using **data scaling** for clustering performance.
- Creating **visual insights** from clustering results.

---

## 👤 Author
**AlaEldin Ali**  

_Data Science Enthusiast | ML Intern @ Elevvo_  

🔗 [LinkedIn](https://www.linkedin.com/in/x3loox) | [GitHub](https://github.com/x3loox)

---

## 📜 License
This project is for **educational purposes** as part of the Elevvo Pathways internship.
