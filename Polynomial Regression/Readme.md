# 📈 Polynomial Regression — Complete Guide & Implementation

This repository contains a full implementation and explanation of **Polynomial Regression**, including data preprocessing, model training, visualization, and evaluation metrics. Polynomial Regression is a powerful extension of Linear Regression used to model **non-linear relationships** between features.

---

## 🔍 **What is Polynomial Regression?**

Polynomial Regression models the target variable (**Y**) as an **nth-degree polynomial** of the input variable (**X**):

[
Y = b_0 + b_1X + b_2X^2 + ... + b_nX^n
]

It is useful when data shows **curved (non-linear)** patterns.

---

## 🧠 **Features of This Project**

✔ Loads dataset using pandas
✔ Selects feature(s) and target variable
✔ Generates polynomial features
✔ Trains Linear Regression on polynomial-transformed data
✔ Evaluates model using R² Score
✔ Visualizes the fitted polynomial curve
✔ Fully customizable degree (2, 3, 4, …)

---

## 📂 **Project Structure**

```
├── diabetes.csv           # Your dataset
├── polynomial_regression.py   # Main code
├── README.md          # Project documentation
```

---

## 🛠 **Technologies Used**

* Python
* NumPy
* Pandas
* Matplotlib
* scikit-learn

---


## 🧪 **Sample Output (Graph)**

The program generates:

* A scatter plot of actual data
* A smooth polynomial curve (degree = 2 by default)

---

## 📊 **Adjusting Polynomial Degree**

Inside the script:

```python
degree = 2   # Change to 3, 4, 5...
poly = PolynomialFeatures(degree)
```

Higher degrees fit more complex curves but may lead to **overfitting**.

---

## ✔ **Evaluation Metric**

The model uses **R² Score** to measure accuracy:

[
R^2 = 1 - \frac{SSR}{SST}
]

Higher values (close to 1) indicate a better fit.

---

## 📘 **Use Cases**

* Stock price modeling
* Growth prediction
* Weather forecasting
* Curve fitting
* Scientific data modeling
