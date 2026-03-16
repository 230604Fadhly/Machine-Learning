# Machine Learning

# Feature Engineering - Machine Learning Preprocessing

Project ini berisi proses **Feature Engineering** yang digunakan sebagai tahap persiapan data sebelum dilakukan proses **Machine Learning Modeling**.

## Dataset

Dataset yang digunakan dalam project ini antara lain:

* California Housing Dataset
* Company Dataset
* Telco Customer Churn Dataset

---

## Feature Engineering Process

### 1. Outlier Handling

Metode yang digunakan: **Interquartile Range (IQR)**

Kolom yang dianalisis:

* MedInc
* HouseAge
* AveRooms
* AveBedrms
* AveOccup

Outlier pada dataset ditangani pada kolom **MedInc** menggunakan metode **IQR**.

---

### 2. Missing Value Handling

Dataset yang digunakan: **company.csv**

Aturan penanganan missing value:

| Data Type   | Method |
| ----------- | ------ |
| Numeric     | Median |
| Categorical | Mode   |

Kolom **Headquarters** memiliki missing value yang kemudian diisi menggunakan metode **modus (mode)**.

---

### 3. Encoding

Encoding dilakukan untuk mengubah data **kategorikal** menjadi **numerik** sehingga dapat digunakan dalam model Machine Learning.

#### One Hot Encoding

Kolom yang digunakan:

* gender

#### Label Encoding

Kolom yang digunakan:

* Partner
* Dependents
* StreamingMovies
* StreamingTV
* TechSupport
* DeviceProtection
* OnlineBackup
* OnlineSecurity
* MultipleLines

#### Mean Encoding

Kolom yang digunakan:

* Contract

Mean encoding dilakukan dengan menghitung **rata-rata nilai dari variabel target (Churn)**.

---

## Libraries Used

Project ini menggunakan beberapa library Python berikut:

```
pandas
numpy
matplotlib
seaborn
scikit-learn
```

---

## Author

**M. Fadhly Andrian**
