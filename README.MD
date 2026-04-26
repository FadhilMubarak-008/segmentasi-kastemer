# 📊 Customer Segmentation using K-Means

## 🧠 Overview

Project ini dibuat untuk memahami bagaimana cara mengelompokkan customer berdasarkan karakteristik mereka menggunakan metode Machine Learning, khususnya **K-Means Clustering**.

Sebagai seseorang yang masih dalam tahap belajar di bidang Data Science, project ini jadi latihan untuk menggabungkan:

* Data Cleaning
* Exploratory Data Analysis (EDA)
* Machine Learning
* Business Insight

Tujuan utamanya bukan cuma bikin model, tapi juga mencoba memahami:

> “Apa makna dari data ini untuk bisnis?”

---

## 🎯 Problem Statement

Bagaimana cara mengelompokkan customer agar perusahaan dapat:

* memahami karakter tiap segmen
* menentukan strategi marketing yang lebih tepat
* meningkatkan potensi revenue

---

## 📁 Dataset

Dataset yang digunakan berisi informasi customer seperti:

* Age
* Gender
* Profession
* Work Experience
* Family Size
* Spending Score

---

## 🛠️ Data Preprocessing

Beberapa langkah yang dilakukan:

* Mengatasi missing values:

  * Numerical → diisi dengan median
  * Categorical → diisi dengan "Unknown"
* Encoding categorical features menggunakan `pd.get_dummies()`
* Feature scaling menggunakan `StandardScaler`

---

## 📊 Exploratory Data Analysis (EDA)

Beberapa insight awal yang ditemukan:

* Customer dengan usia lebih tinggi cenderung memiliki spending lebih tinggi
* Customer yang belum menikah didominasi oleh low spending
* Gender tidak menunjukkan perbedaan signifikan terhadap perilaku spending
* Family size memiliki pengaruh terhadap pola spending

---

## 🤖 Modeling (K-Means Clustering)

* Menggunakan metode **Elbow Method** untuk menentukan jumlah cluster
* Dipilih jumlah cluster = **4** karena penurunan inertia mulai melambat setelah titik tersebut

---

## 🔍 Hasil Clustering

### 🟢 Cluster 0 — General Customers

* Jumlah terbesar
* Didominasi oleh low hingga average spending

👉 Insight:
Segmen ini bisa ditingkatkan melalui strategi upselling

---

### 🔵 Cluster 1 — Low Value Segment

* Spending sangat rendah
* High spender hampir tidak ada

👉 Insight:
Perlu pendekatan promo atau strategi entry-level

---

### 🟡 Cluster 2 — Potential Segment (Small Group)

* Jumlah kecil tapi memiliki proporsi high spending cukup tinggi

👉 Insight:
Segmen ini berpotensi untuk strategi personalized marketing

---

### 🔴 Cluster 3 — Young Low Engagement

* Usia lebih muda
* Spending sangat rendah

👉 Insight:
Fokus pada awareness atau bisa tidak menjadi prioritas utama

---

## 💡 Key Insights

* Age menjadi faktor yang cukup kuat dalam membedakan perilaku customer
* Tidak semua customer memiliki nilai bisnis yang sama
* Segmentasi membantu perusahaan fokus pada target yang lebih tepat

---

## 🚀 What I Learned

Dari project ini, saya belajar bahwa:

* Machine Learning bukan cuma soal model, tapi soal **insight**
* Data preprocessing itu krusial dan bisa mempengaruhi hasil akhir
* Storytelling dari data itu sama pentingnya dengan coding

---

## 🔧 Tools & Libraries

* Python
* Pandas
* Matplotlib / Seaborn
* Scikit-learn

---

## 📌 Future Improvement

* Mencoba jumlah cluster lain (k=5) untuk perbandingan
* Menggunakan PCA untuk visualisasi cluster
* Membuat dashboard interaktif (Streamlit / Power BI)

---

## 🙌 Closing

Project ini masih jauh dari sempurna, tapi jadi langkah awal untuk memahami dunia Data Science secara lebih praktikal.

Kalau kamu juga lagi belajar, semangat ya — kita sama-sama lagi di proses 🚀
