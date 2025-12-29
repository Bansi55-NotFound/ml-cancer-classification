# KMeans Clustering — Diabetes & Blobs Datasets

This project demonstrates **KMeans clustering** on two different datasets to understand when clustering works well and when it does not.

The goal is to build strong intuition around **unsupervised learning**, **elbow method**, and **silhouette score**.

---

## 🧠 Problem Type

- **Unsupervised Learning (Clustering)**
- No target variable (`y`) is used
- The algorithm discovers patterns on its own

---

## 📊 Datasets Used

### 1️⃣ Diabetes Dataset (Real-world data)

- Source: `sklearn.datasets.load_diabetes`
- Features: Medical measurements
- Target column is **removed**
- Dataset is noisy and continuous in nature

### 2️⃣ Blobs Dataset (Synthetic data)

- Source: `sklearn.datasets.make_blobs`
- Number of samples: 500
- Number of true clusters: 4
- Features: 2 (for easy visualization)
- Dataset is intentionally designed for clustering

---

## 🔄 Approach (Common for Both)

1. Load dataset  
2. Remove target column (if present)  
3. Scale features using `StandardScaler`  
4. Use **Elbow Method** to choose number of clusters (K)  
5. Apply **KMeans clustering**  
6. Visualize clusters  
7. Evaluate clustering using **Silhouette Score**  

---

## 📏 Evaluation Methods

### 🔹 Elbow Method
- Plots number of clusters (K) vs inertia
- Helps identify optimal K where improvement slows

### 🔹 Silhouette Score
- Measures how well points fit within their clusters
- Range: -1 to +1
- Higher score = better cluster separation

---

## 📈 Results

### 🔸 Diabetes Dataset
- Elbow curve not very clear
- Silhouette Score ≈ **0.15**
- Clusters overlap heavily

**Interpretation:**  
The diabetes dataset does not naturally form well-separated clusters, which is common in real-world medical data.

---

### 🔸 Blobs Dataset
- Clear elbow at **K = 4**
- Silhouette Score ≈ **0.80**
- Clusters are well separated

**Interpretation:**  
The blobs dataset is ideal for clustering and helps build intuition about how KMeans behaves when its assumptions are satisfied.

---

## 🧠 Key Learnings

- Clustering does **not** use target labels
- Good clustering depends heavily on data structure
- Elbow method helps choose K, but does not guarantee good clusters
- Silhouette score provides quantitative cluster quality
- Same algorithm can perform very differently on different datasets

---

## 🛠 Tech Stack

- Python
- pandas
- NumPy
- scikit-learn
- matplotlib

---

## ✅ Conclusion

This project highlights that **KMeans clustering is highly data-dependent**. While synthetic data with clear structure results in excellent clustering performance, real-world datasets may not always exhibit strong natural clusters. Understanding this distinction is critical for applying unsupervised learning correctly.
