# Classification Algorithms

Classification algorithms are essential in machine learning, enabling models to predict categorical labels for given data points. This note covers four popular classification algorithms: Support Vector Machine (SVM), k-Nearest Neighbors (k-NN), Decision Trees, and Random Forests.

## 1. Support Vector Machine (SVM)

### Overview
- **SVM** is a supervised learning algorithm used for classification and regression tasks.
- It aims to find the optimal hyperplane that separates classes in high-dimensional space.

### Key Concepts
- **Support Vectors**: Data points closest to the hyperplane that influence its position and orientation.
- **Kernel Trick**: Transforms data into higher dimensions to make it easier to classify non-linearly separable data.
  - Common kernels: Linear, Polynomial, Radial Basis Function (RBF), Sigmoid.

### Advantages
- Effective in high-dimensional spaces.
- Works well with a clear margin of separation.

### Disadvantages
- Less effective on very large datasets.
- Sensitive to noise and outliers.

## 2. k-Nearest Neighbors (k-NN)

### Overview
- **k-NN** is a non-parametric, instance-based learning algorithm used for classification and regression.
- It classifies a data point based on the majority class among its \(k\) nearest neighbors.

### Key Concepts
- **Distance Metrics**: Commonly used metrics include:
  - Euclidean distance
  - Manhattan distance
  - Minkowski distance

### Advantages
- Simple and easy to implement.
- No training phase; all computation is done during the prediction phase.

### Disadvantages
- Computationally expensive for large datasets.
- Sensitive to irrelevant features and the choice of \(k\).

## 3. Decision Trees

### Overview
- A **Decision Tree** is a tree-like model used for classification and regression.
- It splits data into branches based on feature values, leading to decisions or classifications at the leaves.

### Key Concepts
- **Entropy**: Measures the impurity of a dataset. Lower entropy indicates a purer dataset.
- **Gini Index**: Another measure of impurity that is used to evaluate splits in the tree.
- **Pruning**: The process of removing branches that have little importance to improve model generalization.

### Advantages
- Easy to interpret and visualize.
- Handles both numerical and categorical data.

### Disadvantages
- Prone to overfitting, especially with complex trees.
- Sensitive to small variations in data.

## 4. Random Forests

### Overview
- **Random Forest** is an ensemble method that combines multiple decision trees to improve classification accuracy.
- It operates by constructing a multitude of decision trees during training and outputs the mode of the classes for classification tasks.

### Key Concepts
- **Bagging**: Bootstrap aggregating, where random samples of the training data are used to train individual trees.
- **Feature Randomness**: Each tree is trained on a random subset of features, enhancing diversity among the trees.

### Advantages
- Reduces overfitting compared to individual decision trees.
- Handles large datasets and maintains accuracy even when a large proportion of data is missing.

### Disadvantages
- More complex and less interpretable than a single decision tree.
- Requires more computational resources.

---

### Conclusion

Understanding these classification algorithms is crucial for selecting the right model for your data. Each algorithm has its strengths and weaknesses, making them suitable for different types of problems and datasets. By experimenting with these methods, you can find the most effective approach for your specific classification tasks.

