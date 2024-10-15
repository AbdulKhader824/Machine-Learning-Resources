# Clustering Algorithms: K-means and DBSCAN

## Introduction
Clustering is an unsupervised machine learning technique used to group similar data points based on specific features. This document covers two widely used clustering algorithms: K-means and DBSCAN.

## K-means Clustering

### Overview
K-means is a partitioning-based clustering algorithm that divides the dataset into K distinct clusters. The algorithm aims to minimize the variance within each cluster.

### Algorithm Steps
1. **Initialization**: Randomly select K centroids from the dataset.
2. **Assignment**: Assign each data point to the nearest centroid, forming K clusters.
3. **Update**: Recalculate the centroids as the mean of the assigned points.
4. **Repeat**: Iterate steps 2 and 3 until convergence (centroids no longer change).

### Choosing the Value of K
- **Elbow Method**: Plot the Within-Cluster Sum of Squares (WCSS) against different K values and look for an "elbow" point where the rate of decrease sharply changes.
- **Silhouette Score**: Calculate the silhouette coefficient for different K values to find the optimal number of clusters.

### Strengths and Weaknesses
- **Strengths**:
  - Simple and easy to implement.
  - Scales well to large datasets.
  
- **Weaknesses**:
  - Requires specifying K in advance.
  - Sensitive to outliers and noise.
  - Assumes spherical clusters.

### Loss Function
- The loss function for K-means is the sum of squared distances between points and their corresponding centroids:
  \[
  L = \sum_{i=1}^{K} \sum_{x_j \in C_i} ||x_j - \mu_i||^2
  \]
  where \( C_i \) is the ith cluster and \( \mu_i \) is the centroid of the ith cluster.

### Handling Missing Data
- **Imputation**: Fill in missing values using methods like mean, median, or more sophisticated techniques.
- **Removal**: Exclude data points with missing values or remove features with many missing values.

### Distance Metrics
- Common distance metrics used in K-means include:
  - **Euclidean Distance**: Measures straight-line distance.
  - **Manhattan Distance**: Measures grid-based distance.
  - **Minkowski Distance**: Generalizes both Euclidean and Manhattan distances.

## DBSCAN (Density-Based Spatial Clustering of Applications with Noise)

### Overview
DBSCAN is a density-based clustering algorithm that groups together points that are closely packed while marking points in low-density regions as outliers.

### Algorithm Steps
1. **Select Parameters**: Define the parameters \( \epsilon \) (the radius) and MinPts (minimum points required to form a dense region).
2. **Identify Core Points**: A point is a core point if it has at least MinPts points within the \( \epsilon \) neighborhood.
3. **Form Clusters**: Connect core points with their neighbors to form clusters. Expand clusters until all points in a neighborhood are classified.
4. **Identify Outliers**: Points that are neither core points nor directly reachable from core points are marked as noise.

### Advantages Over K-means
- **No need to specify the number of clusters in advance**.
- **Can find clusters of arbitrary shape**.
- **Handles noise and outliers effectively**.

### Parameters and Their Influence
- **Epsilon (\( \epsilon \))**: Determines the size of the neighborhood; a smaller \( \epsilon \) may lead to many points being classified as noise.
- **MinPts**: A higher MinPts value requires a denser area to form a cluster.

### Strengths and Weaknesses
- **Strengths**:
  - Robust to noise and outliers.
  - Can discover clusters of varying shapes and sizes.
  
- **Weaknesses**:
  - Requires careful tuning of parameters \( \epsilon \) and MinPts.
  - Struggles with high-dimensional data due to the curse of dimensionality.

### Evaluating Performance
Common methods to evaluate the performance of clustering models include:
- **Silhouette Score**: Measures how similar a point is to its own cluster compared to other clusters.
- **Normalized Mutual Information (NMI)**: Measures the agreement between the clustering results and ground truth labels.
- **Davies-Bouldin Index**: Evaluates the average similarity ratio of each cluster with the cluster that is most similar to it.

## Conclusion
Clustering algorithms like K-means and DBSCAN provide powerful tools for data analysis and pattern recognition. Understanding their strengths, weaknesses, and applications is essential for effectively utilizing these algorithms in real-world scenarios.
