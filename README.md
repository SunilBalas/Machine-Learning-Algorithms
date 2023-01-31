# Machine Learning Algorithms
This document provides a high-level overview of different machine learning algorithms and concepts.

## Supervised Learning
Supervised learning is a type of machine learning where the model learns from labeled data to make predictions about future instances.

1. **Linear Regression** <br>
    - Linear regression is a simple approach for modeling the relationship between a dependent variable and one or more independent variables. The model generates a linear equation to predict the dependent variable.

2. **Logistic Regression** <br>
    - Logistic regression is a type of regression analysis used to predict a categorical dependent variable based on one or more independent variables.

3. **Decision Tree** <br>
    - A decision tree is a flowchart-like structure where each internal node represents a test on an attribute, each branch represents the outcome of the test and each leaf node represents a class label.

4. **Random Forest** <br>
    - A random forest is an ensemble of decision trees, where each tree votes to predict the class of an instance. The final prediction is the average of all the votes.

5. **Support Vector Machine (SVM)** <br>
    - Support Vector Machine (SVM) is a supervised machine learning algorithm that can be used for both classification and regression tasks. The goal of the SVM is to find a hyperplane that separates the data into different classes.

## Unsupervised Learning
Unsupervised learning is a type of machine learning where the model learns from unlabeled data to make predictions about future instances.

1. **K-Means Clustering** <br>
    - K-Means is an iterative algorithm that separates data into K clusters based on their similarity.

## Dummy Variables & One Hot Encoding
  - Dummy variables and one hot encoding are techniques used to convert categorical variables into numerical variables for use in regression or machine learning algorithms.
  - A dummy variable is a binary variable that takes on the value of 1 or 0, indicating the presence or absence of a certain categorical attribute. For example, if a variable represents the color of a car (red, blue, green), three dummy variables would be created with a value of 1 for the respective color and 0 for the others.
 - One hot encoding is a more advanced form of creating dummy variables, where a new column is created for each unique category of a categorical variable. Each row is then marked with a 1 in the column that represents the category it belongs to and 0s in the other columns. One hot encoding is more flexible and less prone to errors compared to creating dummy variables by hand.
 - In Python, both dummy variables and one hot encoding can be easily created using the get_dummies function from the pandas library. Here's an example:
 
   ```python
      import pandas as pd

      # Create a sample dataframe with categorical variable
      df = pd.DataFrame({'color': ['red', 'blue', 'green', 'red']})

      # Create dummy variables
      df_dummies = pd.get_dummies(df['color'])

      # One hot encoding
      df_encoded = pd.get_dummies(df, columns=['color'], prefix='color')

   ```
   
   ## Gradient Descent
    - Gradient descent is a optimization algorithm used to minimize a cost function in machine learning by iteratively updating the parameters of a model in the direction of steepest reduction of the cost.
    - For instance, the algorithm iteratively adjusts the parameters such as weights and biases of the neural network to find the optimal parameters that minimise the loss function.
