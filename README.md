# 🧠 Clustering Data Non-Linear dengan DBSCAN (`make_moons()`)

Repositori ini berisi implementasi dan eksplorasi algoritma **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)**  
menggunakan dataset simulasi `make_moons()` dari pustaka `scikit-learn`. Proyek ini merupakan bagian dari tugas kuliah  
**Kecerdasan Buatan (Artificial Intelligence)** dengan topik **Unsupervised Learning – Clustering**.

---

## 📌 Tujuan Proyek

Tujuan utama dari proyek ini adalah:

- Menerapkan algoritma DBSCAN untuk melakukan klasterisasi data tanpa label (unsupervised)
- Menangani bentuk klaster yang tidak bisa dipisahkan secara linear
- Menggunakan metrik evaluasi untuk menilai kualitas hasil klasterisasi
- Memahami perbedaan antara DBSCAN dan algoritma lain seperti K-Means

---

## 📁 Deskripsi Dataset

Dataset yang digunakan berasal dari fungsi `make_moons()`:

```python
from sklearn.datasets import make_moons
X, y = make_moons(n_samples=500, noise=0.05, random_state=42)
