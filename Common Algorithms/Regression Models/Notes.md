## Common Algorithms: Regression Models

### Linear Regression
- **Definition**: A simple regression algorithm used to predict a continuous dependent variable (Y) based on one or more independent variables (X).
- **How it works**: It fits a line (or a hyperplane in the case of multiple features) that best represents the relationship between the independent and dependent variables. The goal is to minimize the difference between the predicted and actual values using a method called **Least Squares**.
- **Formula**:  
  \[
  Y = \beta_0 + \beta_1X_1 + \beta_2X_2 + ... + \beta_nX_n + \epsilon
  \]
  where:
  - \(Y\) = Dependent variable (target)
  - \(X_1, X_2, ..., X_n\) = Independent variables (features)
  - \(\beta_0, \beta_1, ..., \beta_n\) = Coefficients (weights)
  - \(\epsilon\) = Error term

- **Use Cases**:
  - Predicting housing prices based on features like size, location, and number of rooms.
  - Estimating sales based on factors like advertising spend, product price, etc.

---

### Logistic Regression
- **Definition**: A classification algorithm used when the dependent variable is categorical (e.g., 0 or 1, True or False). Despite its name, it's mainly used for **binary classification** tasks.
- **How it works**: Instead of fitting a straight line (as in Linear Regression), it applies the **logistic (sigmoid) function** to output a probability that the input belongs to a certain class (0 or 1). The probability is then thresholded to make the final classification.
- **Formula**:  
  \[
  P(Y=1|X) = \frac{1}{1 + e^{-(\beta_0 + \beta_1X_1 + ... + \beta_nX_n)}}
  \]
  where:
  - \(P(Y=1|X)\) = Probability that the outcome is 1 (positive class)
  - \(X_1, X_2, ..., X_n\) = Independent variables (features)
  - \(\beta_0, \beta_1, ..., \beta_n\) = Coefficients (weights)

- **Use Cases**:
  - Predicting whether a customer will churn (yes/no).
  - Classifying emails as spam or not spam.
  - Disease prediction (e.g., will a patient develop a condition based on medical factors?).

---

### Key Differences Between Linear and Logistic Regression
- **Linear Regression** is used for predicting continuous outcomes, while **Logistic Regression** is used for binary or categorical classification.
- **Linear Regression** outputs actual values (regression line), while **Logistic Regression** outputs probabilities between 0 and 1 and classifies based on a threshold (e.g., 0.5).
