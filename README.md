# Task 8 – K-Means Clustering for Mall Customer Segmentation

**AI & ML Internship – Unsupervised Learning**

---

##  Objective
The objective of this task is to apply **K-Means Clustering** to perform **unsupervised learning** and segment mall customers into distinct groups based on their shopping behaviors.

---

##  Dataset
- **Name:** Mall Customer Segmentation Dataset  
- **Features Used:**  
  - Annual Income (k$)  
  - Spending Score (1-100)  
- **Goal:** Identify natural clusters of customers for targeted marketing and business insights.

---

##  Tools & Libraries Used
- **Python 3**
- **Pandas** – data loading and manipulation
- **Scikit-learn** – K-Means clustering, scaling, evaluation
- **Matplotlib** – visualization of clusters and elbow method

---

##  Methodology

### 1. Data Preparation
- Loaded dataset
- Selected relevant numerical features: `Annual Income (k$)` and `Spending Score (1-100)`
- Standardized the features using **StandardScaler** to give equal weight to all features

### 2. Finding Optimal K
- Applied the **Elbow Method** by plotting `inertia` vs. number of clusters (K)
- The elbow point indicated an optimal `K = 5`

### 3. Model Training
- Trained **K-Means** model with `n_clusters=5` and `random_state=42`
- Assigned cluster labels to each customer

### 4. Visualization
- Created a scatter plot of the clusters
- Different colors represent different clusters
- Cluster centers marked with `'X'`

### 5. Evaluation
- Calculated **Silhouette Score** to measure cluster separation quality

---

##  How to Run
1. Install dependencies:
   ```bash
   pip install pandas scikit-learn matplotlib
