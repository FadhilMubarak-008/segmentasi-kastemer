# 📊 Segmentasi kastemer dengan menggunakan K-Means

## 1. Overview

Project ini dibuat untuk memahami bagaimana cara mengelompokkan customer berdasarkan karakteristik mereka menggunakan metode Machine Learning, khususnya **K-Means Clustering**.

Disclimer : 

- Saya masih dalam tahap belajar data analis
- Dataset yang digunakan berasal dari kaggle
- Saya menggunakan bantuan AI untuk membantu saya berpikir dalam menganalisis data


Sebagai seseorang yang masih dalam tahap belajar di bidang Data Science dan machine learning, project ini jadi latihan untuk menggabungkan:

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Machine Learning
- Business Insight

Tujuan utamanya bukan cuma bikin model, tapi juga mencoba memahami:

> “Apa makna dari data ini untuk bisnis?”

---

## 2. Problem Statement

Bagaimana cara mengelompokkan customer agar perusahaan dapat:

- memahami karakter tiap segmen
- menentukan strategi marketing yang lebih tepat
- meningkatkan potensi revenue

---

## 3. Dataset

Dataset yang digunakan berisi informasi customer seperti:

- Age
- Gender
- Profession
- Work Experience
- Family Size
- Spending Score

---

## 4. Data Preprocessing

Beberapa langkah yang dilakukan:

- Mengatasi missing values:

  * Numerical → diisi dengan median
  * Categorical → diisi dengan "Unknown"
- Encoding categorical features menggunakan `pd.get_dummies()`
- Feature scaling menggunakan `StandardScaler`

---

## 5. Exploratory Data Analysis (EDA)

Beberapa insight awal yang ditemukan:

- Customer dengan usia lebih tinggi cenderung memiliki spending lebih tinggi
- Customer yang belum menikah didominasi oleh low spending (pengeluarang rendah)
- Gender tidak menunjukkan perbedaan signifikan terhadap perilaku spending
- Family size memiliki pengaruh terhadap pola spending

---

## 6. Modeling (K-Means Clustering)

- Menggunakan metode **Elbow Method** untuk menentukan jumlah cluster
- Dipilih jumlah cluster = **4** karena penurunan inertia mulai melambat setelah titik tersebut

---

## 🔍 Hasil Clustering

###  Cluster 0 — General Customers

- Jumlah terbesar
- Didominasi oleh low hingga average spending

Insight:
Segmen ini bisa ditingkatkan melalui strategi upselling

---

###  Cluster 1 — Low Value Segment

- Spending sangat rendah
- High spender hampir tidak ada

Insight:
Perlu pendekatan promo atau strategi entry-level

---

###  Cluster 2 — Potential Segment (Small Group)

- Jumlah kecil tapi memiliki proporsi high spending cukup tinggi

Insight:
Segmen ini berpotensi untuk strategi personalized marketing

---

###  Cluster 3 — Young Low Engagement

- Usia yang lebih muda
- Spendingnya sangat rendah

Insight:
Fokus pada awareness atau bisa tidak menjadi prioritas utama

---

## Hasil Insights :

- Age menjadi faktor yang cukup kuat dalam membedakan perilaku customer
- Tidak semua customer memiliki nilai bisnis yang sama
- Segmentasi membantu perusahaan fokus pada target yang lebih tepat

---

## Apa yang saya pelajari?

Dari project ini, saya belajar bahwa:

- Sebelum melakukan analisis kita harus tahu tujuan dan apa masalah yang ingin kita selesaikan
- Machine Learning bukan cuma soal model canggih, tapi soal **insight**
- Data preprocessing itu krusial dan bisa mempengaruhi hasil akhir
- Memahami hubungan feature dan target adalah hal yang sangat penting
- Storytelling dari data itu sama pentingnya dengan coding

---

## 🔧 Tools & Libraries yang saya pakai

* Python
* Pandas
* Matplotlib
* Scikit-learn

---

##  Penutup

Project ini masih jauh dari sempurna, tapi menjadi langkah awal untuk memahami dunia Data Science secara lebih mendalam.

Aku sedang dalam proses belajar ☺️
