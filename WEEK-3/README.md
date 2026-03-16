# Exploratory Data Analysis (EDA)

Repository ini berisi proses **Exploratory Data Analysis (EDA)** yang dilakukan sebagai bagian dari pembelajaran **Feature Engineering** dan **Data Preparation** sebelum tahap **Machine Learning Modelling**.

EDA digunakan untuk:

* memahami karakteristik dataset
* mengidentifikasi pola distribusi data
* mendeteksi outlier
* menangani missing value
* melakukan encoding pada variabel kategorikal

---

## Dataset yang Digunakan

Proyek ini menggunakan beberapa dataset sebagai studi kasus:

1. **California Dataset** – digunakan untuk analisis distribusi data dan outlier detection
2. **Company Dataset** – digunakan untuk latihan penanganan missing value
3. **Telco Customer Churn Dataset** – digunakan untuk latihan encoding variabel kategorikal

---

## Tujuan Analisis

Tujuan dari Exploratory Data Analysis pada proyek ini adalah:

1. Memahami struktur dan karakteristik dataset
2. Mengidentifikasi distribusi data
3. Mendeteksi dan menangani outlier
4. Mengidentifikasi dan menangani missing value
5. Mengubah variabel kategorikal menjadi numerikal menggunakan encoding

---

## Tahapan Analisis

### 1. Data Understanding

Tahap awal untuk memahami struktur dataset yang meliputi:

* jumlah data
* tipe data setiap kolom
* statistik deskriptif

Library yang digunakan:

* pandas
* numpy

---

### 2. Analisis Distribusi Data

Distribusi data dianalisis menggunakan beberapa metode visualisasi:

* Histogram
* Q-Q Plot
* Boxplot

Visualisasi ini membantu memahami pola distribusi serta mendeteksi adanya **outlier**.

Library yang digunakan:

* matplotlib
* seaborn
* scipy

---

### 3. Handling Outlier

Outlier dideteksi menggunakan metode **Interquartile Range (IQR)**.

Rumus yang digunakan:

IQR = Q3 − Q1

Lower Bound = Q1 − 1.5 × IQR

Upper Bound = Q3 + 1.5 × IQR

Data yang berada di luar batas tersebut dianggap sebagai **outlier** dan kemudian dilakukan **capping** (penggantian nilai dengan batas maksimum atau minimum).

---

### 4. Missing Value Handling

Missing value dianalisis berdasarkan persentase data yang hilang.

Aturan yang digunakan:

* Jika missing value **> 20%** → kolom dihapus
* Jika missing value **≤ 20%** → dilakukan imputasi

Untuk data kategorikal digunakan metode **modus (mode)**.

---

### 5. Encoding

Encoding dilakukan untuk mengubah variabel kategorikal menjadi numerikal agar dapat digunakan dalam algoritma machine learning.

Metode encoding yang digunakan:

* **One Hot Encoding (OHE)** → kolom `Gender`
* **Label Encoding / Ordinal Encoding** → kolom `Partner`, `Dependents`
* **Mean Encoding** → kolom `Contract`

---

## Teknologi yang Digunakan

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy
* Scikit-learn
