
# K-Means Clustering

## 📌 Overview

K-Means Clustering is an **unsupervised machine learning algorithm** used to group data points into **K distinct clusters** based on feature similarity. Each cluster is represented by its **centroid** (mean of the points in that cluster).

The algorithm aims to **minimize intra-cluster variance** (sum of squared distances between points and their respective centroids).

---

## 🧠 Intuition

* Data points that are **close to each other** should belong to the same cluster
* Each cluster has a **center (centroid)**
* Points are repeatedly reassigned until clusters stabilize

---

## ⚙️ How K-Means Works

1. Choose the number of clusters **K**
2. Randomly initialize **K centroids**
3. Assign each data point to the **nearest centroid** (usually using Euclidean distance)
4. Recalculate centroids as the **mean of assigned points**
5. Repeat steps 3–4 until:

   * Centroids do not change, or
   * Maximum iterations are reached

---

## 📐 Distance Metric

Most commonly used:

[ \text{Euclidean Distance} = \sqrt{(x_1-x_2)^2 + (y_1-y_2)^2} ]

Other metrics (less common): Manhattan, Cosine

---

## ⏱️ Time & Space Complexity

* **Time Complexity:** `O(n × k × d × i)`

  * `n` = number of data points
  * `k` = number of clusters
  * `d` = number of dimensions
  * `i` = number of iterations

* **Space Complexity:** `O(n + k)`

---

## 📊 Choosing the Right K

### Elbow Method

* Plot **K vs Inertia (WCSS)**
* Choose K where the decrease slows ("elbow")

### Silhouette Score

* Measures how similar a point is to its own cluster vs others
* Range: `-1 to 1`

---

## ✅ Advantages

* Simple and easy to implement
* Fast and scalable for large datasets
* Works well when clusters are clearly separated

---

## ❌ Limitations

* Must predefine **K**
* Sensitive to initial centroid placement
* Struggles with:

  * Non-spherical clusters
  * Different cluster sizes
  * Outliers

---

## 🧪 Example

Input data points:

```
(1,2), (1,4), (1,0), (10,2), (10,4), (10,0)
```

With `K = 2`, the algorithm will form two clusters around `(1,2)` and `(10,2)`.

---

## 🛠️ Applications

* Customer segmentation
* Image compression
* Document clustering
* Market basket analysis
* Pattern recognition

---

## 📦 Requirements

* Python / C++ / Java (any language)
* Libraries (optional):

  * `numpy`, `matplotlib`, `scikit-learn`

---

## 📚 References

* MacQueen, J. (1967). *Some Methods for Classification and Analysis of Multivariate Observations*
* Scikit-learn Documentation

---

## ✨ Notes

* Standardize data before applying K-Means
* Run multiple initializations (`k-means++`) for better results

---

**Author:** Paras Rajput
