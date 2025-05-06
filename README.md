# K-Means-Clustering

This project is a part of the **AI & ML Internship** program. The objective of this task is to apply **K-Means Clustering** (an unsupervised machine learning algorithm) on the **Mall Customers dataset** to segment customers based on their purchasing behavior.



## 📌 Objective

To perform unsupervised learning using the K-Means algorithm to:

- Identify distinct customer groups based on `Annual Income` and `Spending Score`.
- Visualize the clustering results.
- Evaluate clustering quality using the **Elbow Method** and **Silhouette Score**.



## 🗃️ Dataset

**File Name**: `Mall_Customers.csv`

**Description**:  
The dataset contains information about customers including:

- CustomerID
- Gender
- Age
- Annual Income (k$)
- Spending Score (1-100)

For clustering, we used only the **Annual Income (k$)** and **Spending Score (1-100)** columns.



## 🛠️ Tools & Libraries Used

- Python 3.x
- [Pandas](https://pandas.pydata.org/)
- [Matplotlib](https://matplotlib.org/)
- [Seaborn](https://seaborn.pydata.org/)
- [Scikit-learn](https://scikit-learn.org/)



## 📈 Implementation Steps

### 1. Load and Inspect the Dataset
- Loaded the dataset using Pandas.
- Displayed basic info and selected relevant features.

### 2. Preprocessing
- Scaled the selected features (`Annual Income` and `Spending Score`) using `StandardScaler` for better K-Means performance.

### 3. Elbow Method for Optimal K
- Calculated **inertia** (within-cluster sum of squares) for K from 1 to 10.
- Plotted the Elbow Curve.
- Found the **optimal number of clusters** to be around **K = 5**.

### 4. Apply K-Means Clustering
- Initialized and fit the `KMeans` model with `n_clusters=5`.
- Added the predicted cluster labels to the dataset.

### 5. Cluster Visualization
- Visualized the clusters using:
  - A 2D scatter plot (Annual Income vs Spending Score)
  - PCA-based scatter plot for future extension to higher-dimensional data

### 6. Evaluation
- Computed the **Silhouette Score** to evaluate clustering performance.



## 📊 Results

- **Optimal number of clusters (k):** 5
- **Silhouette Score:** ~0.55 (indicating moderately good clustering)
- Clear visual separation between customer segments in the 2D plots


## 💾 Files in the Repository

| File | Description |
|------|-------------|
| `Mall_Customers.csv` | Original dataset |
| `K_Means_Clustering.ipynb` | Python script for K-Means clustering |
| `README.md` | Detailed project documentation |


## ✅ Conclusion

This task demonstrated how K-Means can be used for customer segmentation based on spending behavior, which can help businesses make data-driven marketing decisions.

