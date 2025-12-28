# KMeans Clustering on Diabetes Dataset

This project applies **KMeans clustering** on the sklearn Diabetes dataset to explore whether the data naturally forms clusters.

## Problem Type
- Unsupervised Learning (Clustering)
- No target variable is used

## Dataset
- sklearn Diabetes dataset
- Only feature columns are used
- Target column is intentionally excluded

## Approach
1. Load dataset
2. Remove target column
3. Scale features using StandardScaler
4. Use Elbow Method to choose number of clusters
5. Apply KMeans clustering
6. Evaluate clustering using Silhouette Score

## Evaluation
- **Elbow Method**: Used to select an appropriate number of clusters
- **Silhouette Score**: Used to evaluate cluster quality

## Result
- Silhouette Score ≈ 0.15

## Interpretation
The low silhouette score indicates overlapping clusters, suggesting that the diabetes dataset does not naturally form well-separated groups. This is expected for medical datasets and demonstrates that not all datasets are suitable for clustering.

## Key Learning
- Clustering does not always produce strong groups
- Low silhouette score does not mean incorrect implementation
- Understanding data suitability is critical in unsupervised learning

## Tech Stack
- Python
- pandas
- scikit-learn
- matplotlib
