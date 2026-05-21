# Customer-Segmentation-RFM-Analysis-K-means-Clustering

This project aims to segment customers based on their purchasing behavior using **RFM (Recency, Frequency, Monetary)** analysis combined with **KMeans Clustering**. The goal is to help businesses better understand their customers and develop more targeted marketing strategies. This project also generates monthly reports and stores the data in a database for future analysis.

---

## 📊 Dataset

The dataset used in this project is an online retail dataset from UCI Machine Learning. The dataset is a transactional data that contains transactions from December 1st 2010 until December 9th 2011 for a UK-based online retail.

---

## 📌 Objectives

- Create and store Monthly Reports Dataset using Spark SQL
- Visualiza data to gain insights
- Perform data cleaning and preprocessing  
- Create RFM features for customer behavior profiling
- Use PCA (Principal Component Analysis) to transform data into fewer variables  
- Identify the optimal number of clusters using metrics like **Elbow Method**, **Silhouette Score**, and **Davies-Bouldin Index**  
- Apply **KMeans clustering** for customer segmentation  
- Analyze each segment for actionable business insights  
- Visualize customer segments using radar charts and plots

---

## ⚙️ Methodology

### 1. Data Cleaning & Preprocessing
- Handle missing values
- Remove duplicate and invalid transactions

### 2. Feature Engineering (RFM)
- **Recency**: Days since last purchase  
- **Frequency**: Total number of transactions  
- **Monetary**: Total spending
- Add other features to check customer behavior

### 3. Data Modeling
- Normalize RFM values
- PCA (Principal Component Analysis)
- Determine optimal **K** using:
  - Elbow Method
  - Silhouette Score
  - Davies-Bouldin Index
- Apply **KMeans Clustering**

### 4. Data Evaluation & Insights
- Interpret cluster characteristics
- Visualize using **Radar Charts**
- Provide recommendations per segment

---

## 📈 Key Results

- Optimal number of clusters found: **K = 3**
- Cluster 1: Low spenders, active on weekends
  <img width="639" height="578" alt="image" src="https://github.com/user-attachments/assets/30178b2a-3b87-4871-a328-2f1d587392f5" />

- Cluster 2: Inactive customers

  
- Cluster 3: High-value customers – frequent, high spending

Notes: The model can still be improved to create clusters that are more distinctly separated.
For example by experimenting with different clustering parameters or algorithms to reduce similarities in certain customer characteristics.

---

## 💡 Business Recommendation

- Offer loyalty programs or discounts to Cluster 1 to increase spending  
- Re-engage Cluster 2 via personalized promotions  
- Reward Cluster 3 with premium benefits to ensure retention

---

## 🛠️ Tech Stack

- Python  
- Pandas, NumPy  
- Scikit-learn  
- Plotly 
- Google Colab
- Spark SQL

