# Assignment 6 - K-Means Clustering pada Wine Quality Dataset

## Informasi Mahasiswa
**Nama:** M. Fadhly Andrian  
**NIM:** 4222311015  
**Kelas:** Robotika A Malam  
**Mata Kuliah:** RE603 Machine Learning  

---

## Deskripsi Project
Project ini merupakan implementasi algoritma **K-Means Clustering** menggunakan **Wine Quality Dataset**.

Tujuan dari assignment ini adalah:
- Melakukan preprocessing data
- Melakukan normalisasi fitur
- Menerapkan algoritma K-Means
- Menentukan cluster terbaik
- Melakukan visualisasi hasil clustering menggunakan PCA
- Menganalisis karakteristik masing-masing cluster

---

## Dataset
Dataset yang digunakan:

**Wine Quality Dataset (WineQT.csv)**

Dataset berisi beberapa atribut kimia dari wine, seperti:

- Fixed acidity
- Volatile acidity
- Citric acid
- Residual sugar
- Chlorides
- Free sulfur dioxide
- Total sulfur dioxide
- Density
- pH
- Sulphates
- Alcohol
- Quality

---

## Library yang Digunakan

Project ini menggunakan beberapa library Python berikut:

```python
pandas
numpy
matplotlib
scikit-learn
```

Install dependency:

```bash
pip install pandas numpy matplotlib scikit-learn
```

---

## Tahapan Pengerjaan

### 1. Import Library
Mengimpor library yang dibutuhkan untuk analisis data dan clustering.

---

### 2. Load Dataset
Dataset dibaca menggunakan:

```python
pd.read_csv('WineQT.csv')
```

---

### 3. Preprocessing Data
Melakukan:
- Pembersihan data
- Pemilihan fitur
- Persiapan data untuk clustering

---

### 4. Normalisasi Data
Menggunakan **StandardScaler** agar seluruh fitur memiliki skala yang sama.

```python
StandardScaler()
```

---

### 5. Clustering Menggunakan K-Means
Model clustering dibangun menggunakan:

```python
KMeans()
```

Digunakan untuk mengelompokkan data wine berdasarkan karakteristiknya.

---

### 6. Evaluasi Cluster
Evaluasi kualitas cluster dilakukan menggunakan:

- **Silhouette Score**

Tujuan evaluasi:
- Menentukan jumlah cluster optimal
- Mengukur kualitas pemisahan cluster

---

### 7. Visualisasi Menggunakan PCA
Dimensi data direduksi menjadi 2 komponen utama menggunakan:

```python
PCA(n_components=2)
```

Kemudian divisualisasikan dalam scatter plot.

---

### 8. Analisis Hasil
Melakukan analisis rata-rata tiap cluster menggunakan:

```python
df.groupby('Cluster').mean()
```

Hal ini digunakan untuk melihat karakteristik masing-masing kelompok wine.

---

## Cara Menjalankan

Jalankan notebook:

```bash
jupyter notebook Assignment6.ipynb
```

atau jika menggunakan VS Code:

- Buka file `Assignment6.ipynb`
- Jalankan setiap cell secara berurutan

---

## Output
Program menghasilkan:

- Data hasil clustering
- Nilai evaluasi silhouette score
- Visualisasi scatter plot clustering
- Rata-rata karakteristik tiap cluster

---

## Kesimpulan
Algoritma **K-Means Clustering** berhasil digunakan untuk mengelompokkan data wine berdasarkan karakteristik kimianya.

Dengan bantuan **PCA**, hasil clustering dapat divisualisasikan secara lebih mudah untuk dianalisis.
