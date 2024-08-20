# Introduction to Supervised Learning in Python

## Chapter 1: Foundations of Supervised Learning

### Lesson 1.1: Supervised Learning Basics
- Learner will be able to define supervised learning and distinguish it from unsupervised learning.
- Learner will be able to distinguish between regression and classification tasks and understand their real-world applications.
- Learner will have a high-level understanding of the workflow of building a supervised learning model.

### Lesson 1.2: Exploratory Data Analysis (EDA) and Preprocessing
- Learner will be able to identify different types of variables using pandas.
- Learner will be able to explore summary statistics of numerical variables, handle missing values, and encode categorical variables.
- Functions introduced:
  - pandas: `read_csv()`, `DataFrame.describe()`, `DataFrame.info()`, `isnull()`, `dropna()`, `fillna()`
  - sklearn.preprocessing: `LabelEncoder()`
  - sklearn.impute: `SimpleImputer()`

### Lesson 1.3: Data Visualization
- Learner will be able to create histograms to understand data distributions.
- Learner will be able to create scatterplots to identify potential linear and non-linear relationships.
- Functions introduced:
  - matplotlib.pyplot: `hist()`, `scatter()`

## Chapter 2: Regression

### Lesson 2.1: Simple Linear Regression
- Learner will be able to build a simple linear regression model.
- Learner will be able to interpret the coefficients and intercept of a linear regression model.
- Learner will be able to evaluate the performance of a simple linear regression model by calculating and interpreting R-squared and RMSE.
- Functions introduced:
  - sklearn.linear_model: `LinearRegression()`
  - LinearRegression methods: `fit()`, `predict()`, `score()`
  - sklearn.metrics: `mean_squared_error()`, `r2_score()`

### Lesson 2.2: Multiple Linear Regression
- Learner will be able to build a multiple linear regression model based on correlation analysis.
- Learner will be able to interpret the coefficients of a multiple linear regression model.
- Learner will be able to compare the performance of simple and multiple linear regression models using R-squared and RMSE.
- Functions introduced:
  - pandas: `DataFrame.corr()`
  - seaborn: `heatmap()`

### Lesson 2.3: Polynomial Regression
- Learner will be able to explain when linear models might not be suitable for a given dataset.
- Learner will be able to leverage insights from data visualization to inform model choice (linear vs polynomial).
- Learner will be able to implement polynomial regression to capture non-linear relationships.
- Learner will be able to visualize underfitting with low-degree polynomials and overfitting with high-degree polynomials.
- Learner will be able to interpret the trade-off between model complexity and generalization.
  - sklearn.preprocessing: `PolynomialFeatures()`

## Chapter 3: Classification

### Lesson 3.1: Logistic Regression
- Learner will be able to implement logistic regression for binary classification.
- Learner will be able to interpret the coefficients of a logistic regression model.
- Learner will be able to evaluate the performance of a logistic regression model using accuracy.
- Functions introduced:
  - sklearn.linear_model: `LogisticRegression()`
  - sklearn.metrics: `accuracy_score()`

### Lesson 3.2: K-Nearest Neighbors (KNN) Classification
- Learner will develop a high-level understanding of how KNN algorithm works.
- Learner will be able to implement the KNN algorithm for binary classification.
- Learner will be able to explain the effect of the number of neighbors (K) on model performance.
- Functions introduced:
  - sklearn.neighbors: `KNeighborsClassifier()`

### Lesson 3.3: Decision Trees
- Learner will be able to build and visualize a simple decision tree classifier.
- Learner will be able to explain the basic concepts of decision trees and tree structure (e.g., information gain, Gini impurity).
- Learner will be able to interpret a decision tree's structure and make predictions.
- Functions introduced:
  - sklearn.tree: `DecisionTreeClassifier()`, `plot_tree()`

## Chapter 4: Model Evaluation and Improvement

### Lesson 4.1: Additional Evaluation Metrics
- Learner will be able to explain why accuracy and RMSE alone may not always be sufficient for model evaluation.
- Learner will be able to calculate and interpret other metrics such as Mean Absolute Error (MAE) for regression tasks and precision and recall for classification tasks.
- Learner will be able to create and interpret a basic confusion matrix.
- Functions introduced:
  - sklearn.metrics: `mean_absolute_error()`
  - sklearn.metrics: `precision_score()`, `recall_score()`, `confusion_matrix()`

### Lesson 4.2: Train-test Split
- Learner will be able to explain the importance of splitting data for training and testing.
- Learner will be able to implement a basic train-test split and evaluate models using a holdout test set for both regression and classification tasks.
- Learner will be able to define and distinguish between overfitting and underfitting (first introduced in 2.3).
- Learner will be able to recognize signs of overfitting (high training accuracy, low test accuracy) and underfitting (underfitting (low accuracy on both training and test sets).
- Functions introduced:
  - sklearn.model_selection: `train_test_split()`

### Lesson 4.3: Cross-Validation
- Learner will be able to describe the concept of cross-validation and its benefits over a single train-test split.
- Learner will be able to implement k-fold cross-validation for regression and classification.
- Learner will be able to interpret cross-validation scores.
- Functions introduced:
  - sklearn.model_selection: `KFold()`, `cross_val_score()`

### Lesson 4.4: Strategies for Model Improvement
- Learner will be able to explain basic strategies to address underfitting (e.g., increasing model complexity) and overfitting (e.g., simplifying the model).
- Learner will be able to describe regularization as a technique to prevent overfitting.
- Learner will be able to implement Ridge regression as an example of regularization.
- Learner will be able to use basic hyperparameter tuning using a GridSearch to adjust the regularization strength in Ridge regression and assess its impact on model performance.
- Learner will be able to discuss how hyperparameter tuning can be applied to other models.
- Functions introduced:
  - sklearn.linear_model: Ridge()
  - sklearn.model_selection: `GridSearchCV()`
