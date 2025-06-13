# 🧠 DBSCAN Clustering on `make_moons()` Dataset

This repository contains an implementation of **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)** using the popular `make_moons()` dataset from scikit-learn.  
It demonstrates how DBSCAN can effectively separate non-linear clusters and detect outliers.

---

## 📌 Project Overview

- **Goal**: Apply DBSCAN to non-linear data (`make_moons`) and evaluate clustering quality
- **Method**: Density-based clustering (DBSCAN)
- **Evaluation**: Visual inspection + Adjusted Rand Index (ARI)

---

## 📁 Dataset

Using synthetic data generated from:

```python
from sklearn.datasets import make_moons
X, y = make_moons(n_samples=500, noise=0.05, random_state=42)
