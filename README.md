# 📌 DBSCAN - Density-Based Spatial Clustering of Applications with Noise

## 📖 Overview

**DBSCAN** is a powerful **density-based clustering algorithm** that groups together data points that are closely packed, marking points in low-density regions as **outliers**. Unlike k-means, it does **not require the number of clusters to be specified in advance** and can find arbitrarily shaped clusters.

## 🔍 Key Concepts

* **Epsilon (ε)**: Radius for neighborhood search.
* **MinPts**: Minimum number of points required to form a dense region.
* **Core Point**: A point with at least `MinPts` neighbors within `ε`.
* **Border Point**: Has fewer than `MinPts` neighbors but is in the neighborhood of a core point.
* **Noise (Outlier)**: Any point that is neither a core point nor a border point.

## ⚙️ How DBSCAN Works

1. Pick an unvisited point.
2. If it has ≥ `MinPts` neighbors within distance `ε`, form a new cluster.
3. Recursively expand the cluster by including density-reachable points.
4. Mark remaining points as noise.

## ✅ Advantages

* Does **not** require the number of clusters.
* Can find **arbitrarily shaped** clusters.
* Handles **noise** effectively.
* Robust to outliers.

## ❌ Limitations

* Struggles with clusters of **varying density**.
* Sensitive to `ε` and `MinPts`.
* Less effective in **high-dimensional** data.

## 📦 Applications

* Spatial data analysis
* Anomaly detection
* Image processing
* Market segmentation
* Pattern recognition


## 📘 References

* [Original Paper (Ester et al., 1996)](https://www.aaai.org/Papers/KDD/1996/KDD96-037.pdf)
* [Scikit-learn Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html)

---

Would you like a version formatted as a GitHub-style `README.md` file?
