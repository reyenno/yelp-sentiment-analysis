# Yelp Sentiment Analysis with Apache Spark

## 📌 Deskripsi
Proyek ini mengimplementasikan **Analisis Sentimen** pada dataset ulasan Yelp menggunakan **Apache Spark (PySpark)** sebagai Big Data tool dan **Machine Learning** untuk klasifikasi sentimen pelanggan.

Dataset yang digunakan adalah **Yelp Open Dataset** yang berisi **6.9 juta ulasan** restoran dan bisnis dari berbagai kota di Amerika Serikat, dengan ukuran file **4.98 GB**.

---

## 🎯 Tujuan
- Menganalisis sentimen ulasan pelanggan (Positif/Negatif)
- Membandingkan performa dua algoritma Machine Learning
- Mengidentifikasi pola perilaku pelanggan dari data berskala besar

---

## 🛠️ Teknologi yang Digunakan
| Komponen | Tools |
|---|---|
| Big Data Processing | Apache Spark (PySpark) |
| Machine Learning | PySpark MLlib |
| Visualisasi | Matplotlib, Seaborn, WordCloud |
| Environment | Google Colab |
| Dataset | Yelp Open Dataset (Kaggle) |

---

## 📊 Dataset
- **Sumber:** [Yelp Dataset - Kaggle](https://www.kaggle.com/datasets/yelp-dataset/yelp-dataset)
- **File:** `yelp_academic_dataset_review.json`
- **Ukuran:** 4.98 GB
- **Total Reviews:** 6,990,280
- **Kolom utama:** `stars`, `text`, `date`, `useful`, `funny`, `cool`

---

## 🤖 Model Machine Learning
Dua model dibandingkan dalam proyek ini:

| Model | AUC-ROC | Akurasi | F1-Score |
|---|---|---|---|
| Logistic Regression | **0.9778** | **91.95%** | **0.9159** |
| Naive Bayes | 0.6238 | 88.79% | 0.8896 |

**Kesimpulan:** Logistic Regression unggul di semua metrik karena mampu menangkap hubungan kompleks antar fitur TF-IDF, sementara Naive Bayes mengasumsikan setiap fitur independen sehingga kurang optimal untuk data teks.

---

## 📈 Visualisasi
1. Distribusi Rating Bintang Yelp Reviews
2. Proporsi Sentimen Ulasan
3. Rata-rata Panjang Review berdasarkan Sentimen
4. Tren Review & Sentimen per Tahun
5. Word Cloud Review Positif & Negatif
6. Perbandingan Performa Model

---

## 🚀 Cara Menjalankan

### Prerequisites
- Akun Google (untuk Google Colab)
- Akun Kaggle (untuk download dataset)

### Langkah-langkah
1. Buka notebook di Google Colab
2. Jalankan Cell 1 untuk install library
3. Masukkan Kaggle API Token di Cell 3
4. Jalankan semua cell secara berurutan

### Struktur Notebook
| Cell | Keterangan |
|---|---|
| Cell 1 | Install library |
| Cell 2 | Import semua library |
| Cell 3 | Setup Kaggle API |
| Cell 4 | Download & ekstrak dataset |
| Cell 5 | Inisialisasi PySpark & load data |
| Cell 6 | Preprocessing & labeling |
| Cell 7 | Pipeline AI & training model |
| Cell 8 | Evaluasi kedua model |
| Cell 9 | Visualisasi & analisis |

---

## 📁 Struktur Repository
```
yelp-sentiment-analysis/
│
├── Sentiment_Analysis_Yelp.ipynb   # Notebook utama
├── README.md                        # Dokumentasi proyek
└── LICENSE                          # MIT License
```

---

## 👤 Author
**reyenno**  
Mata Kuliah: Artificial Intelligence dan Big Data
