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

- 500 data titik, fitur `x1`, `x2`
- Label hanya untuk evaluasi

## 🔧 Tahapan dan Teknologi

1. Generate data dengan `make_moons()`
2. Normalisasi menggunakan `StandardScaler`
3. DBSCAN: `eps=0.3`, `min_samples=5`
4. Visualisasi hasil
5. Evaluasi menggunakan **Adjusted Rand Index (ARI)**

Teknologi:
- Python 3.x
- `numpy`, `pandas`, `matplotlib`, `seaborn`, `scikit-learn`

## 📈 Hasil dan Evaluasi

- Cluster 0: 250 data
- Cluster 1: 250 data
- Outlier: 0 data
- ARI: 1.00 ✅ (clustering sempurna)

## 🖼️ Visualisasi

![Hasil Clustering DBSCAN](./7a04f96e-a487-483f-97b7-1e89c798923a.png)

## ▶️ Cara Menjalankan

```bash
git clone https://github.com/username-kamu/dbscan-clustering-moons.git
cd dbscan-clustering-moons
pip install numpy pandas matplotlib seaborn scikit-learn
python dbscan_moons.py
```

## 🎯 Penjelasan DBSCAN

- Mengelompokkan berdasarkan kepadatan titik (density)
- Tidak butuh jumlah klaster dari awal
- Bisa deteksi noise / outlier
- Lebih fleksibel untuk data bentuk bebas
