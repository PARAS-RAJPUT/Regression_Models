# K-Fold Cross Validation

## 📌 Overview

**K-Fold Cross Validation** is a powerful model evaluation technique used in machine learning to assess how well a model generalizes to unseen data. Instead of using a single train-test split, the dataset is divided into **K equal-sized folds**, and the model is trained and validated **K times**, each time using a different fold as the validation set.

This approach provides a more reliable estimate of model performance, especially when working with limited data.

---

## 🔁 How K-Fold Cross Validation Works

1. Split the dataset into **K folds** of roughly equal size.
2. For each iteration `i = 1 to K`:

   * Use the `i-th` fold as the **validation set**.
   * Use the remaining `K-1` folds as the **training set**.
3. Train the model and record the evaluation metric.
4. Compute the **average performance** across all K iterations.

```
Dataset → Split into K folds
For each fold:
    Train on K-1 folds
    Validate on 1 fold
Final Score = Average of K results
```

---

## ⚙️ Key Parameters

* **K (Number of Folds)**: Common values are 5 or 10
* **Shuffle**: Whether to shuffle data before splitting
* **Random State**: Ensures reproducibility

---

## 🧠 Why Use K-Fold Cross Validation?

* Reduces bias from a single train-test split
* Makes efficient use of limited data
* Provides a more stable and reliable evaluation
* Helps detect overfitting

---

## 🛠️ Types of K-Fold Validation

* **Standard K-Fold** – Randomly splits data into K folds
* **Stratified K-Fold** – Preserves class distribution (used in classification)
* **Group K-Fold** – Ensures groups are not split across folds
* **Time Series Split** – Maintains temporal order (not random)

---

## 🧪 Example (Conceptual)

Suppose K = 5:

* Fold 1 → Validation, Folds 2–5 → Training
* Fold 2 → Validation, Folds 1,3–5 → Training
* ...
* Fold 5 → Validation, Folds 1–4 → Training

Each data point is used:

* Once for validation
* K−1 times for training

---

## 📊 Evaluation Metrics

Common metrics used with K-Fold:

* Accuracy
* Precision, Recall, F1-score
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R² Score

Final metric = **Mean ± Standard Deviation** across folds

---

## ⚠️ Advantages

* Better generalization estimate
* Less variance in performance metrics
* Suitable for small to medium datasets

---

## ❌ Limitations

* Computationally expensive for large datasets
* Not ideal for time-series data (unless modified)
* Training time increases by a factor of K

---

## 🔮 Best Practices

* Use **Stratified K-Fold** for classification problems
* Shuffle data when appropriate
* Choose K carefully (higher K → higher computation)
* Combine with hyperparameter tuning (GridSearchCV)

---

## 🚀 Applications

* Model evaluation and comparison
* Hyperparameter tuning
* Preventing overfitting
* Academic and research experiments

---

## 📚 Tools & Libraries

* **scikit-learn** (KFold, StratifiedKFold)
* TensorFlow / Keras


---

## 📜 License

This project/documentation is provided under the **MIT License**.

---

## ✨ Author

**Paras Rajput**

If this README helped you, consider giving the project a ⭐!

