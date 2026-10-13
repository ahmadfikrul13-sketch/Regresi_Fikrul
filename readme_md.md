# 📊 Analisis Regresi Linear: Faktor Kemiskinan di Kota Bandung

Proyek ini bertujuan untuk menganalisis pengaruh alokasi/belanja daerah di sektor **Pendidikan** dan **Kesehatan** terhadap **Tingkat Kemiskinan** di Kota Bandung menggunakan metode **Regresi Linear (Time Series)** periode **2014 – 2024**.

---

## 📌 Deskripsi Variabel

Dalam analisis ini, variabel yang digunakan adalah sebagai berikut:

* **Variabel Dependen ($Y$)**:
  * **`KEMISKINAN`**: Tingkat atau persentase kemiskinan di Kota Bandung.
* **Variabel Independen ($X$)**:
  * **`bm_pendidikan` ($X_1$)**: Alokasi / Belanja Modal Bidang Pendidikan.
  * **`bm_kesehatan` ($X_2$)**: Alokasi / Belanja Modal Bidang Kesehatan.
* **`Tahun`**: Periode data pengamatan (*Time Series*, 2014–2024, total 11 observasi).

---

## 📂 Struktur Repositori

```text
.
├── Data/                 # Dataset (Excel/CSV)
├── Notebooks/            # Jupyter Notebook (.ipynb)
├── README.md             # Dokumentasi proyek
└── requirements.txt      # Dependency / Library Python
```

---

## 🛠️ Persyaratan & Instalasi

Untuk menjalankan notebook ini secara lokal, pastikan Anda telah menginstal **Python 3.x** dan library pendukung berikut:

### 1. Clone Repositori
```bash
git clone https://github.com/username/regresi-kemiskinan-bandung.git
cd regresi-kemiskinan-bandung
```

### 2. Install Library Dependency
```bash
pip install -r requirements.txt
```

Library utama yang digunakan:
* `pandas` & `numpy` - Manipulasi dan analisis data
* `statsmodels` & `scikit-learn` - Pemodelan Regresi Linear & Uji Asumsi Klasik
* `matplotlib` & `seaborn` - Visualisasi data dan grafik residual

---

## 📈 Metodologi & Tahapan Analisis

1. **Exploratory Data Analysis (EDA)**:
   * Analisis deskriptif variabel.
   * Visualisasi tren kemiskinan, belanja pendidikan, dan belanja kesehatan (2014–2024).
2. **Uji Asumsi Klasik**:
   * **Uji Normalitas**: Memastikan residual berdistribusi normal.
   * **Uji Multikolinearitas (VIF)**: Memastikan tidak ada korelasi kuat antar variabel bebas ($X_1$ dan $X_2$).
   * **Uji Heteroskedastisitas**: Memastikan varians residual konstan.
   * **Uji Autokorelasi**: Menguji korelasi antar observasi runtut waktu.
3. **Pemodelan Regresi Linear**:
   * Estimasi Parameter $\beta_0, \beta_1, \beta_2$.
   * Formulasi model:
     $$\text{Kemiskinan} = \beta_0 + \beta_1(\text{bm\_pendidikan}) + \beta_2(\text{bm\_kesehatan}) + \epsilon$$
4. **Evaluasi Model**:
   * **Uji F** (Simultan) & **Uji t** (Parsial).
   * Koefisien Determinasi ($R^2$ & *Adjusted* $R^2$).

---

## 📊 Ringkasan Hasil Utama

*(Isi bagian ini sesuai dengan temuan akhir notebook Anda)*

* **Pengaruh Belanja Pendidikan ($X_1$)**: [Jelaskan secara singkat signifikansi & arah hubungannya]
* **Pengaruh Belanja Kesehatan ($X_2$)**: [Jelaskan secara singkat signifikansi & arah hubungannya]
* **Nilai $R^2$**: Model mampu menjelaskan sebesar **XX%** variasi tingkat kemiskinan di Kota Bandung.

---

## 👥 Kontributor

* **[Nama Anda]** - *Data Analyst / Author* - [GitHub Profile](https://github.com/username)

---
*Dokumen ini dibuat untuk kepentingan analisis data dan keterbukaan riset publik.*