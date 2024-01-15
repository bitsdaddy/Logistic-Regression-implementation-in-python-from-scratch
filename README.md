# Logistic-Regression-implementation-in-python-from-scratch

Logistic Regression is a fundamental algorithm used for binary classification tasks. Unlike linear regression, which predicts continuous values, logistic regression predicts the probability of an observation belonging to a particular class.

## Key Concepts:

### 1. Sigmoid Function:

- Logistic Regression uses the sigmoid (logistic) function to squash the output of a linear equation between 0 and 1.
- The sigmoid function is defined as $( \sigma(z) = \frac{1}{1 + e^{-z}} )$, where $\ z $ is a linear combination of input features and weights.

### 2. Hypothesis Function:

- The hypothesis function for logistic regression is $( h_\theta(x) = \sigma(\theta^Tx) )$, where $ \theta $ represents the weights and $ x $ represents the input features.

### 3. Training Process:

- Logistic regression is trained using an iterative optimization algorithm, commonly gradient descent.
- The objective is to minimize a cost function that measures the difference between the predicted probabilities and the actual class labels.
- The cost function is defined as: 
  $$ J(\theta) = -\frac{1}{m} \sum_{i=1}^{m} [y^{(i)}\log(h_\theta(x^{(i)})) + (1 - y^{(i)})\log(1 - h_\theta(x^{(i)}))] $$

### 4. Decision Boundary:

- The decision boundary is the line that separates the different classes in the feature space.
- It is determined by the weights learned during the training process.

## Code Explanation:

The provided code demonstrates a custom implementation of logistic regression using gradient descent. Here's a breakdown of the key components:

- **Data Preprocessing:**
  - The dataset is loaded and preprocessed by encoding categorical variables (Gender) and dropping unnecessary columns.
- **Visualizations:**
  - Scatter plots are used to visualize relationships between features and the target variable.
- **Logistic Regression Implementation:**
  - The custom logistic regression function is defined, which involves calculating predictions using the sigmoid function and updating weights through gradient descent.
  - The sigmoid function is given by $( \sigma(z) = \frac{1}{1 + e^{-z}} )$.
- **Model Evaluation:**
  - The model is applied to the dataset, and accuracy is calculated to assess its performance.
- **Comparison with Scikit-learn:**
  - The accuracy of the custom logistic regression model is compared with scikit-learn's logistic regression implementation.
