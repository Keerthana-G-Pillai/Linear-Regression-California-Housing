<div align="center">

# 🏠 California Housing Price Prediction

### Simple Linear Regression with One Variable

📊 **Machine Learning Laboratory — Experiment 1**

---

*A simple implementation of Linear Regression to explore the relationship between average rooms and median house values using the California Housing Dataset.*

</div>

## 🎯 Objective

To implement **Linear Regression with one variable** on the **California Housing Dataset** and understand how a linear model learns the relationship between an input feature and a target variable.

---

## 📊 Dataset

The experiment uses the **California Housing Dataset**, which contains information about housing districts in California.

|     | Variable        | Description                           |
| --- | --------------- | ------------------------------------- |
| 🏘️ | **AveRooms**    | Average number of rooms per household |
| 💰  | **MedHouseVal** | Median house value                    |

> **AveRooms** is used as the input feature to predict **MedHouseVal**.

---

## 🔄 Experiment Workflow

**Load Dataset** → **Select Feature** → **Split Data** → **Train Model** → **Optimize Parameters** → **Make Predictions** → **Visualize Results**

---

## 🧠 Concepts Explored

### 📈 Simple Linear Regression

Simple Linear Regression models the relationship between a **single independent variable** and a **dependent variable** by fitting the best possible straight line through the data.

In this experiment, the model learns the relationship between the **average number of rooms** and the **median house value**.

### 📉 Cost Function

The cost function measures how far the model's predictions are from the actual house values.

A **lower cost** indicates that the model's predictions are closer to the actual values.

### 🔄 Gradient Descent

Gradient Descent is used to gradually adjust the model parameters and minimize the cost function.

With each iteration, the model attempts to reduce its prediction error until the cost converges toward a minimum value.

---

## 📉 Cost Convergence Curve

The **Cost Convergence Curve** visualizes how the cost changes during Gradient Descent.

📌 A decreasing curve shows that the model is learning.

📌 A curve that gradually becomes flat indicates that Gradient Descent is converging.

This visualization helps verify whether the optimization process is working correctly.

---

## 📈 Regression Line Visualization

The **Regression Line** shows the relationship learned by the Linear Regression model.

* 🟣 **Data Points** — Actual house values
* 🟢 **Regression Line** — Predicted relationship between average rooms and house value

The visualization makes it easier to understand how well the linear model represents the actual data.

---

## 🛠️ Technologies Used

| Technology              | Purpose                              |
| ----------------------- | ------------------------------------ |
| 🐍 **Python**           | Programming and model implementation |
| 🔢 **NumPy**            | Numerical computations               |
| 📊 **Matplotlib**       | Data visualization                   |
| 🤖 **Scikit-learn**     | California Housing Dataset           |
| 📓 **Jupyter Notebook** | Interactive development              |

---

## ✨ Key Learnings

✔️ Understanding the fundamentals of Simple Linear Regression
✔️ Working with a real-world housing dataset
✔️ Selecting a single feature for prediction
✔️ Understanding the role of the Cost Function
✔️ Optimizing model parameters using Gradient Descent
✔️ Analyzing model convergence
✔️ Visualizing predictions using a Regression Line

---

## ✅ Result

The **Simple Linear Regression model** was successfully implemented using the California Housing Dataset.

The **Cost Convergence Curve** demonstrates how the prediction error decreases during training, while the **Regression Line Visualization** illustrates the relationship between the average number of rooms and median house values.

---

<div align="center">

### 🏡 From Data to Predictions 📈

**Linear Regression • Gradient Descent • Machine Learning**

</div>
