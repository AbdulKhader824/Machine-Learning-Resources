# Supervised, Unsupervised, and Reinforcement Learning

## Supervised Learning
- **Definition**: The model learns from labeled data (input-output pairs) to make predictions.
- **Key Concepts**: 
  - Labeled data
  - Model learns mapping from input to output
- **Examples**:
  - **Classification**: Spam detection (e.g., email is spam or not).
  - **Regression**: Predicting house prices.
- **Use Cases**:
  - Object detection, sentiment analysis, speech recognition.
- **Common Algorithms**:
  - Linear Regression, Support Vector Machines (SVM), Random Forests.

## Unsupervised Learning
- **Definition**: The model works with **unlabeled data** to find hidden patterns.
- **Key Concepts**: 
  - Unlabeled data
  - Model discovers data structures (e.g., clustering)
- **Examples**:
  - **Clustering**: Grouping customers by behavior.
  - **Dimensionality Reduction**: PCA to reduce dataset complexity.
- **Use Cases**:
  - Market segmentation, anomaly detection, data visualization.
- **Common Algorithms**:
  - K-means, Hierarchical Clustering, Principal Component Analysis (PCA).

## Reinforcement Learning (RL)
- **Definition**: The model (agent) interacts with an environment and learns through **rewards** and **penalties**.
- **Key Concepts**: 
  - Agent, Environment, Actions, Rewards
  - Exploration vs. Exploitation
- **Examples**:
  - Game-playing (e.g., AlphaGo)
  - Robotics, self-driving cars.
- **Use Cases**:
  - Decision-making in uncertain environments.
- **Common Algorithms**:
  - Q-Learning, Deep Q-Networks (DQN), Policy Gradient Methods.

## Comparison Table

|               | Supervised Learning                    | Unsupervised Learning                | Reinforcement Learning             |
|---------------|----------------------------------------|--------------------------------------|-----------------------------------|
| **Goal**      | Learn mapping from input to output     | Discover hidden patterns             | Maximize cumulative reward        |
| **Data**      | Labeled data                           | Unlabeled data                       | Feedback via interaction          |
| **Feedback**  | Direct (correct output known)          | No direct feedback                   | Reward or penalty based on actions|
| **Examples**  | Classification, Regression             | Clustering, Dimensionality Reduction | Game playing, Robotics            |
| **Algorithms**| SVM, Neural Networks                   | K-Means, PCA                         | Q-learning, Policy Gradients      |
