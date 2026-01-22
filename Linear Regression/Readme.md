# Linear Regression on Student Performance (Kaggle Dataset)

This README provides a complete guide for building a **Linear Regression model** using the **Student Performance Dataset** from Kaggle. The dataset contains attributes related to student demographics, study habits, parental background, and academic performance. The aim is to predict student scores using regression techniques.

---

## 📌 Project Overview

The objective of this project is to develop a predictive model that estimates **student final scores** based on various input features such as study time, number of absences, parental education, and more. Linear Regression is used as the primary model.

---

## 📂 Dataset Information

* **Source:** Kaggle — Student Performance Dataset
* **Files:** `student-mat.csv`, `student-por.csv` (depending on the version)
* **Target Variable:** `G3` (Final grade)
* **Other Key Features:**

  * `G1` (First period grade)
  * `G2` (Second period grade)
  * `studytime`
  * `failures`
  * `absences`
  * `health`
  * `schoolsup`, `famsup`, `internet`

---

## 🛠️ Technologies & Libraries Used

* Python 3.x
* Pandas
* NumPy
* Scikit-learn
* Matplotlib / Seaborn
* Jupyter Notebook

---

## 📊 Workflow Steps

### **1. Importing Libraries**

Load necessary ML and data analysis tools.

### **2. Loading the Dataset**

```python
df = pd.read_csv('student-mat.csv')
df.head()
```

### **3. Exploratory Data Analysis (EDA)**

* Checking missing values
* Statistical summary (`df.describe()`)
* Understanding distribution of scores
* Correlation heatmap to identify strongly related features

### **4. Feature Selection**

Most correlated predictors:

* `G1` and `G2` (strongest predictors of `G3`)
* `studytime`
* `failures`
* `absences`
* `schoolsup` / `famsup` / `internet`

### **5. Data Preprocessing**

* Encoding categorical variables using `LabelEncoder`
* Handling missing values (if any)
* Feature scaling using `StandardScaler`

### **6. Train-Test Split**

```python
from sklearn.model_selection import train_test_split
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
```

---

## 🤖 Model Development

### **Linear Regression Model**

```python
from sklearn.linear_model import LinearRegression
model = LinearRegression()
model.fit(X_train, y_train)
```

### **Predictions**

```python
pred = model.predict(X_test)
```

---

## 📈 Model Evaluation Metrics

The following metrics are used:

* **MAE** (Mean Absolute Error)
* **MSE** (Mean Squared Error)
* **RMSE** (Root Mean Squared Error)
* **R² Score**

Example:

```python
from sklearn.metrics import mean_squared_error, r2_score
mse = mean_squared_error(y_test, pred)
rmse = mse**0.5
r2 = r2_score(y_test, pred)
```

Expected results (approximate):

* R² Score: **0.80–0.90** (G1 & G2 give strong linear relationship)
* RMSE: Low error if grades correlate strongly

---

## 📊 Visualizations

* Distribution of grades (G1, G2, G3)
* Heatmap showing correlation between features
* Actual vs Predicted score comparison plot
* Residual plot to check linear regression assumptions

---

## 📁 Project Structure

```
|-- data/
|   └── student-mat.csv
|-- notebooks/
|   └── linear_regression_student_performance.ipynb
|-- src/
|   └── model.py
|-- README.md
```

---

## 📝 How to Run the Project

1. Install the dependencies:

```bash
pip install -r requirements.txt
```

2. Open the notebook:

```bash
jupyter notebook linear_regression_student_performance.ipynb
```

3. Run all cells.

---

## 🚀 Possible Improvements

* Use **Polynomial Regression** for complex patterns
* Apply **Regularization (Lasso/Ridge)** to reduce overfitting
* Feature engineering (combine study variables, parent education)
* Hyperparameter tuning

---

## 🤝 Contributing

Pull requests are welcome. You can enhance the model, improve feature engineering, or add visualizations.

---

## 📧 Contact

If you want help customizing this README further or setting up notebooks, feel free to ask
on E Mail : parasrajput987045@gmail.com

