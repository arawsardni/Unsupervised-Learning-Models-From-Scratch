# Unsupervised-Learning-Models-From-Scratch

# 📊 Customer Segmentation using Unsupervised Learning

> **Disclaimer**: The provided Jupyter Notebook and detailed project documentation are written in **Bahasa Indonesia**.

This project is part of the **Advanced Artificial Intelligence** coursework at Universitas Brawijaya. It focuses on customer segmentation using **unsupervised learning algorithms** to uncover hidden patterns and group customers with similar characteristics. The dataset is obtained from the [Kaggle Customer Segmentation Dataset](https://www.kaggle.com/datasets/vetrirah/customer).

## 📌 Project Goals

* Implement **K-Means Clustering** and **Agglomerative Hierarchical Clustering** (single linkage & complete linkage) both manually and using libraries.
* Optimize clustering performance using **Principal Component Analysis (PCA)** for dimensionality reduction.
* Determine the optimal number of clusters using the **Elbow Method** and *Silhouette Score*.
* Evaluate clustering quality using internal metrics (Silhouette Score, Davies-Bouldin Index, Calinski-Harabasz Index) and external metrics (Adjusted Rand Index, Purity Score).
* Analyze the characteristics of each resulting customer segment to support targeted marketing strategies.

## 🛠 Tools & Libraries

* Python
* Pandas & NumPy (data manipulation)
* Matplotlib & Seaborn (visualization)
* Scikit-learn (preprocessing, PCA, KMeans, AgglomerativeClustering, evaluation)
* Custom manual implementation of K-Means and Hierarchical Clustering (single & complete linkage, Euclidean & Manhattan distance metrics)

## 📈 Methods

### 1. Data Preprocessing

* Dropped irrelevant columns (`ID`, `Var_1`).
* Removed outliers using the IQR method.
* Handled missing values (median for numerical, mode for categorical & binary).
* Encoding:

  * Label Encoding for binary features.
  * Ordinal Encoding for `Spending_Score`.
  * One-Hot Encoding for `Profession`.
* Corrected skewness with logarithmic transformation.
* Feature scaling with StandardScaler.
* Stratified sampling to improve computational efficiency for manual hierarchical clustering.
* Applied PCA for dimensionality reduction and visualization.

### 2. Modeling

* **K-Means Clustering**:

  * Manual implementation using Euclidean distance.
  * Scikit-learn implementation (`KMeans`).
* **Agglomerative Hierarchical Clustering**:

  * Manual implementation of *single linkage* and *complete linkage* (Euclidean & Manhattan).
  * Scikit-learn implementation (`AgglomerativeClustering`).

### 3. Evaluation

* **Internal Metrics**: Silhouette Score, Davies-Bouldin Index, Calinski-Harabasz Index.
* **External Metrics**: Adjusted Rand Index, Purity Score.
* Performance comparison and analysis of resulting clusters.

## 🔍 Key Findings

* The **optimal number of clusters** determined by both the Elbow Method and Silhouette Score is **4**, aligning with the original segmentation from the marketing team.
* **K-Means** produced the best performance on internal metrics, while hierarchical clustering provided structural insights into data relationships.
* **PCA** significantly improved computational efficiency and enhanced cluster visualization without losing essential information.
* The resulting segmentation can be used to design more personalized and effective marketing strategies.

## 👨‍🏫 Authors

* Gaung Taqwa Indraswara (235150207111043)
* Muhammad Fauzan (235150201111044)
* Ferrel Destatiananda Edwardo (235150207111044)
* Muhammad Fatir Zaira (23515020011039)

## 📚 Advisor

* Putra Pandu Adikara, S.Kom., M.Kom.

## 🏫 Institution

Faculty of Computer Science, Universitas Brawijaya
Course: Advanced Artificial Intelligence
Year: 2025
