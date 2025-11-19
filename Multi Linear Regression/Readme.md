# Multiple Linear Regression Model – Kaggle Housing Dataset

This project demonstrates **Multiple Linear Regression (MLR)** using the **Boston Housing dataset** from Kaggle.
The goal is to predict the **Median House Value (MEDV)** based on multiple features such as crime rate, number of rooms, population stats, etc.

---

## 📌 Project Objective

* Build a **Multiple Linear Regression** model.
* Perform **Label Encoding** and **OneHotEncoding**.
* Train-test split for model evaluation.
* Visualize:

  * Scatter plot
  * Heatmap
  * Residual heatmap
* Evaluate model performance using:

  * R² Score
  * MSE
  * RMSE

---

## 📂 Dataset

Dataset used: **Boston Housing Dataset**

* **Source:** Kaggle
* **Target Variable:** `MEDV` (Median value of owner-occupied homes)
* **Features:**
  Includes numerical and categorical variables such as:

  * CRIM
  * ZN
  * INDUS
  * CHAS
  * RM
  * AGE
  * TAX
  * PTRATIO
  * LSTAT
  * And more

---

## 🧠 Techniques Used

### ✔ Multiple Linear Regression

Used to model the relationship between multiple independent variables and one dependent variable.

### ✔ Label Encoding

Used for converting the categorical `CHAS` column into numerical values.

### ✔ OneHotEncoding

Used to convert categorical variables into binary columns for regression.

### ✔ Train-Test Split

Dataset divided into **80% training** and **20% testing**.

---

## 🛠 Steps Performed

1. Imported dataset
2. Selected features (X) and target variable (y)
3. Performed Label Encoding on categorical column
4. Applied OneHotEncoding
5. Split data into training and testing sets
6. Trained the Multiple Linear Regression model
7. Made predictions
8. Calculated and printed model accuracy (R² Score)
9. Generated multiple plots:

   * Scatter plot
   * Correlation heatmap

---

## 📈 Model Evaluation

The model was evaluated on:

* **R² Score** → Measures how well independent variables explain the variance in target
* **Mean Squared Error (MSE)**
* **Root Mean Squared Error (RMSE)**

Higher R² and lower MSE/RMSE indicate a better model.

---

## 📊 Visualizations

* **Scatter Plot** (Actual vs Predicted)
* **Heatmap** (Feature Correlation)

These visualizations help understand model accuracy and error distribution.

---



## 👤 Author

**Paras Rajput**

Feel free to contribute or ask for enhancements!


