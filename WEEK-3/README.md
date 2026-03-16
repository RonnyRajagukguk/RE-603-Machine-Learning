\# Exploratory Data Analysis (EDA)



\## Deskripsi Proyek



Proyek ini berisi proses \*\*Exploratory Data Analysis (EDA)\*\* yang dilakukan untuk memahami karakteristik data sebelum digunakan dalam proses \*\*machine learning modelling\*\*. Tahapan analisis meliputi pengecekan distribusi data, penanganan outlier, penanganan missing value, serta proses encoding pada variabel kategorikal.



Dataset yang digunakan pada proyek ini antara lain:



\* \*\*California Dataset\*\*

\* \*\*Company Dataset\*\*

\* \*\*Telco Customer Churn Dataset\*\*



Analisis dilakukan menggunakan \*\*Python\*\* dengan bantuan beberapa library data science.



\---



\## Tujuan Analisis



Tujuan dari Exploratory Data Analysis pada proyek ini adalah:



\* Memahami struktur dan karakteristik dataset

\* Mengidentifikasi distribusi data

\* Mendeteksi dan menangani \*\*outlier\*\*

\* Mengidentifikasi dan menangani \*\*missing value\*\*

\* Melakukan \*\*encoding\*\* pada variabel kategorikal agar dapat digunakan dalam model machine learning



\---



\## Tahapan Analisis



\### 1. Data Understanding



Melakukan eksplorasi awal dataset untuk mengetahui:



\* jumlah data

\* tipe data setiap kolom

\* statistik deskriptif



Library yang digunakan:



\* pandas

\* numpy



\---



\### 2. Analisis Distribusi Data



Distribusi data dianalisis menggunakan beberapa visualisasi:



\* \*\*Histogram\*\*

\* \*\*Q-Q Plot\*\*

\* \*\*Boxplot\*\*



Visualisasi ini membantu dalam memahami pola distribusi data serta mendeteksi adanya outlier.



Library yang digunakan:



\* matplotlib

\* seaborn

\* scipy



\---



\### 3. Handling Outlier



Outlier dideteksi menggunakan metode \*\*Interquartile Range (IQR)\*\*.



Rumus IQR:



\* IQR = Q3 − Q1

\* Lower Bound = Q1 − 1.5 × IQR

\* Upper Bound = Q3 + 1.5 × IQR



Nilai yang berada di luar batas tersebut dianggap sebagai outlier dan kemudian dilakukan \*\*capping\*\* (penggantian nilai dengan batas maksimum atau minimum).



\---



\### 4. Missing Value Handling



Missing value dianalisis berdasarkan persentase data yang hilang.



Aturan yang digunakan:



\* Jika missing value \*\*> 20%\*\* → kolom dihapus

\* Jika missing value \*\*≤ 20%\*\* → dilakukan imputasi



Untuk data kategorikal digunakan metode \*\*modus (mode)\*\*.



\---



\### 5. Encoding



Encoding dilakukan untuk mengubah variabel kategorikal menjadi numerikal sebelum digunakan pada proses machine learning.



Metode encoding yang digunakan:



\* \*\*One Hot Encoding\*\* → pada kolom `Gender`

\* \*\*Label Encoding / Ordinal Encoding\*\* → pada kolom `Partner` dan `Dependents`

\* \*\*Mean Encoding\*\* → pada kolom `Contract`



\---



\## Teknologi yang Digunakan



\* Python

\* Pandas

\* NumPy

\* Matplotlib

\* Seaborn

\* SciPy

\* Scikit-learn



\---



\## Struktur Repository



```

.

├── Assignment\_Week\_3.ipynb

├── california\_dataset.csv

├── company.csv

├── TelcoCustomerChurn.csv

└── README.md

```



\---



\## Kesimpulan



Melalui proses Exploratory Data Analysis, data dapat dipahami dengan lebih baik sebelum digunakan dalam proses pemodelan machine learning. Tahapan seperti penanganan outlier, missing value, dan encoding sangat penting untuk meningkatkan kualitas data serta performa model yang akan dibangun.



