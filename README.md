# Insurance-Cross-Sell-XGBoost
Predicting health insurance customer interest in vehicle insurance using XGBoost Classifier. Achieved 0.85 ROC-AUC score.
[![Python](https://img.shields.io)](https://www.python.org)
[![XGBoost](https://img.shields.io)](https://xgboost.readthedocs.io)
[![License: MIT](https://img.shields.io)](https://opensource.org)

## 📌 Deskripsi Proyek
Proyek ini bertujuan untuk memprediksi apakah nasabah asuransi kesehatan yang sudah ada tertarik untuk membeli **Asuransi Kendaraan**. Dengan menggunakan model ini, perusahaan dapat mengoptimalkan kampanye pemasaran dengan menargetkan nasabah yang memiliki probabilitas konversi tinggi, sehingga menghemat biaya operasional (telemarketing).

## 📊 Hasil Model (2026 Benchmark)
Berdasarkan pengujian pada data test, model **XGBoost** berhasil mencapai performa sebagai berikut:
- **ROC-AUC Score:** `0.8579` (Kategori: Sangat Bagus)
- **Recall (Target 1):** `0.92` (Model berhasil menangkap 92% calon pembeli potensial)

## 💡 Temuan Utama (Business Insights)
Setelah melakukan analisis data (EDA) dan Feature Importance, ditemukan beberapa poin kunci:
1. **Kerusakan Kendaraan:** Nasabah yang kendaraannya pernah rusak sebelumnya memiliki minat beli **5x lebih tinggi**.
2. **Status Asuransi:** Nasabah yang **belum** memiliki asuransi kendaraan sebelumnya adalah target utama (konversi tertinggi).
3. **Umur Kendaraan:** Kendaraan berusia 1-2 tahun ke atas lebih cenderung diasuransikan kembali oleh nasabah dibanding kendaraan baru (<1 tahun).

## 🛠️ Tech Stack & Workflow
- **Pandas:** Manipulasi data & cleaning.
- **Matplotlib & Seaborn:** Visualisasi data.
- **XGBoost:** Algoritma machine learning utama dengan penanganan *imbalanced data* menggunakan parameter `scale_pos_weight`.
- **Scikit-Learn:** Evaluasi model & data splitting.

---
**Disclaimer:** Dataset ini bersifat publik dan diambil dari [Kaggle Health Insurance Cross Sell Prediction](https://www.kaggle.com).

