# Train-Test Split & Linear Regression Model

##  Project Overview

This project demonstrates how to build a simple Machine Learning model using **Linear Regression** and evaluate its performance using the **Train-Test Split** method.

The main goal is to understand how a model learns from training data and performs predictions on unseen test data.

---

##  Concepts Covered

* Train-Test Split
* Linear Regression
* Model Training (`fit`)
* Prediction (`predict`)
* Data Preprocessing

---

## Technologies Used

* Python 
* Pandas
* NumPy
* Matplotlib
* Scikit-learn

---

## Workflow

1. **Load Dataset**

2. **Split Data**

   * Training Data (70%)
   * Testing Data (30%)

3. **Train Model**

   * Using Linear Regression

4. **Make Predictions**

   * Predict values using test data

5. **Evaluate Model**

   * Compare predicted vs actual values

---

##  Code Example

```python
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression

# Split data
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=10)

# Train model
model = LinearRegression()
model.fit(X_train, y_train)

# Predict
predictions = model.predict(X_test)
```

---

## Key Insight
* The model learns patterns from training data.
* It is tested on unseen data to evaluate real-world performance.
* This helps avoid overfitting and ensures better generalization.

