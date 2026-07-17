# Linear Regression with One Variable on California Housing Dataset

## Experiment 1

### Aim

To implement **Linear Regression with one variable** on the **California Housing Dataset** and analyze the model using the **cost convergence curve** and **regression line visualization**.

---

## Description

This experiment demonstrates the implementation of **Simple Linear Regression**, where a single input feature is used to predict the target variable.

The **Average Number of Rooms (`AveRooms`)** is used as the independent variable to predict the **Median House Value (`MedHouseVal`)**.

The experiment includes:

* Loading the California Housing Dataset
* Selecting a single feature for regression
* Splitting the dataset into training and testing sets
* Implementing Linear Regression
* Applying Gradient Descent
* Tracking the cost function during training
* Visualizing the cost convergence curve
* Making predictions on test data
* Visualizing the regression line

---

## Dataset

The **California Housing Dataset** contains information about housing districts in California.

For this experiment:

* **Input Feature (X):** Average number of rooms (`AveRooms`)
* **Target Variable (y):** Median house value (`MedHouseVal`)

The target values represent median house values in units of **$100,000**.

---

## Technologies Used

* Python
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook

---

## Linear Regression

Linear Regression finds the relationship between an independent variable `X` and a dependent variable `y` by fitting a straight line to the data.

For one variable, the hypothesis function is:

`h(x) = θ₀ + θ₁x`

Where:

* `θ₀` = Intercept
* `θ₁` = Slope or coefficient
* `x` = Input feature
* `h(x)` = Predicted value

---

## Cost Function

The cost function measures the error between the actual and predicted values.

The Mean Squared Error based cost function is:

`J(θ) = (1 / 2m) Σ(h(x) - y)²`

The objective of Gradient Descent is to minimize this cost.

---

## Gradient Descent

Gradient Descent is an optimization algorithm used to find the optimal values of the model parameters.

During each iteration, the parameters are updated to reduce the cost function.

As Gradient Descent progresses, the cost should decrease and eventually converge to a minimum value.

---

## Cost Convergence Curve

The cost convergence curve plots the cost against the number of Gradient Descent iterations.

```python
plt.figure(figsize=(7,5))
plt.plot(cost_history, color='teal', linewidth=4)
plt.title("Gradient Descent Cost Convergence Curve")
plt.xlabel("Iterations")
plt.ylabel("Cost J(theta)")
plt.grid(True, linestyle='--', alpha=0.6)
plt.show()
```

A decreasing curve indicates that Gradient Descent is successfully minimizing the cost function. When the curve becomes nearly flat, the algorithm has converged.

---

## Regression Line Visualization

The regression line is plotted along with the actual test data.

```python
# Sort X values for a smooth line
index = np.argsort(X_test.flatten())

plt.figure(figsize=(8,5))
plt.scatter(X_test, y_test, color='purple', label="Actual Data")

plt.plot(
    X_test.flatten()[index],
    y_pred_ne[index],
    color='teal',
    linewidth=2,
    label="Regression Line"
)

plt.title("Linear Regression")
plt.xlabel("Average Rooms")
plt.ylabel("Median House Value")
plt.legend()
plt.grid(True)
plt.show()
```

In the visualization:

* The **scatter points** represent the actual house values.
* The **regression line** represents the values predicted by the Linear Regression model.
* The X-axis represents the **Average Number of Rooms**.
* The Y-axis represents the **Median House Value**.

---

## Results

The Linear Regression model was successfully implemented using a single feature from the California Housing Dataset.

The **cost convergence curve** demonstrates how the cost decreases over multiple iterations of Gradient Descent.

The **regression line visualization** shows the relationship between the average number of rooms and median house values and compares the predicted regression line with the actual data points.

---

## Conclusion

This experiment demonstrates the working of **Simple Linear Regression** using the California Housing Dataset. Gradient Descent is used to minimize the cost function and optimize the model parameters. The cost convergence curve helps verify the convergence of the algorithm, while the regression line provides a visual representation of the relationship between the selected feature and the target variable.
