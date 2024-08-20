**Evaluating Model Performance (Part of Lesson 4.3)**

As a data scientist at a credit card company, you're developing a model to predict customer defaults. To ensure your model is stable, you need to evaluate its performance across different subsets of data. Cross-validation is a powerful technique for this purpose, providing a reliable estimate of your model's performance.

`LogisticRegression` has been imported for you from `sklearn.linear_model`, `cross_val_score` from `sklearn.model_selection`, and `numpy` has been imported as `np`. 
The dataset has been stored as `credit_data`, with the columns `age`, `income`, `loan`, and `default`.

**Instructions**
* Split the data into features (X) and target (y).
* Create a logistic regression model.
* Perform 5-fold cross-validation.
* Calculate and print the mean and standard deviation of the cross-validation scores.

```python
# Split the data into features and target
X = credit_data.drop(columns=['____'])
y = credit_data['____']

# Create the logistic regression model
model = ____()

# Perform 5-fold cross-validation
cv_scores = ____(model, X, y, cv=____, scoring='accuracy')

# Calculate mean and standard deviation of scores
mean_score = ____(cv_scores)
std_score = ____(cv_scores)

# Print the results (rounded to two decimal places)
print("Mean accuracy:", round(____, 2))
print("Standard deviation:", round(____, 2))
```
