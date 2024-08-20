**Evaluating Model Performance**

You want to ensure your model's performance is stable across different subsets of your data. In this exercise, you'll use cross-validation to evaluate a logistic regression model.

You have a dataset `credit_data` for credit card default prediction with the following columns:
- 'income': Annual income of the customer
- 'age': Age of the customer
- 'loan': Total loan amount
- 'default': Target variable (1 if defaulted, 0 if not defaulted)

`LogisticRegression` has been imported for you from `sklearn.linear_model`, `cross_val_score` from `sklearn.model_selection`, and `numpy` has been imported as `np`. The dataset has been stored as `credit_data`.

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
