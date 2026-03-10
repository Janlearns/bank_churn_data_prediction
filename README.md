# Bank Churn Data Prediction

## Deskripsi Proyek

Proyek ini bertujuan untuk menganalisis data churn pelanggan bank menggunakan teknik machine learning. Dengan memanfaatkan dataset pelanggan, proyek ini membangun model prediktif untuk mengidentifikasi pelanggan yang berpotensi berhenti menggunakan layanan bank, sehingga memungkinkan perusahaan untuk menerapkan strategi retensi yang efektif.

## Tujuan Program

- Mengembangkan model klasifikasi untuk memprediksi churn pelanggan.
- Mengidentifikasi faktor-faktor utama yang mempengaruhi churn melalui analisis eksplorasi data (EDA).
- Mengevaluasi performa model menggunakan metrik seperti Recall, F1-Score, dan ROC-AUC.
- Mensimulasikan dampak bisnis dari penerapan model, termasuk potensi penghematan revenue melalui strategi retensi.

## Penjelasan Cara Kerja Utama

Kode Python ini melakukan serangkaian langkah analisis data:
1. **Business Understanding**: Menghitung churn rate dan estimasi dampak revenue.
2. **Exploratory Data Analysis (EDA)**: Analisis churn berdasarkan variabel kategorikal seperti usia, tenure, dan frekuensi kontak.
3. **Feature Engineering**: Encoding fitur kategorikal, transformasi fitur numerik dengan StandardScaler, dan penghapusan fitur yang tidak relevan.
4. **Pemodelan Machine Learning**: Pelatihan model menggunakan algoritma Random Forest dan XGBoost dengan optimasi hyperparameter menggunakan Optuna.
5. **Evaluasi Model**: Perbandingan performa model, analisis confusion matrix, dan metrik tambahan.
6. **Analisis Interpretabilitas**: Identifikasi fitur penting menggunakan feature importance dari model XGBoost.
7. **Simulasi Dampak Bisnis**: Estimasi potensi revenue yang diselamatkan melalui retensi pelanggan berisiko tinggi.

## Cara Instalasi dan Dependensi

Pastikan Python 3.7+ terinstal di sistem Anda. Instal dependensi yang diperlukan menggunakan pip:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn optuna xgboost
```

Dependensi utama:
- `pandas`: Manipulasi dan analisis data.
- `numpy`: Operasi numerik.
- `seaborn` dan `matplotlib`: Visualisasi data.
- `scikit-learn`: Algoritma machine learning dan preprocessing.
- `optuna`: Optimasi hyperparameter.
- `xgboost`: Algoritma XGBoost untuk klasifikasi.

## Cara Menjalankan Program

1. Pastikan file dataset `bank_churn_data.csv` tersedia di direktori yang sesuai (sesuai path dalam kode, misalnya `/content/drive/MyDrive/bootcamp/hari_37/bank_churn_data.csv` atau sesuaikan path lokal).


Program akan menjalankan seluruh proses dari pemuatan data hingga simulasi dampak bisnis, dengan output berupa metrik evaluasi dan visualisasi.

## Struktur Kode dan Fungsi Penting

- **Business Understanding**: Fungsi untuk menghitung churn rate dan estimasi revenue loss.
- **EDA**: Analisis distribusi churn berdasarkan variabel seperti usia, tenure, dan kontak.
- **Feature Engineering**: Encoding dan scaling fitur untuk persiapan modeling.
- **Modeling**: Fungsi optimasi hyperparameter dengan Optuna dan pelatihan model Random Forest serta XGBoost.
- **Evaluation**: Perhitungan metrik evaluasi dan visualisasi confusion matrix.
- **Interpretability**: Ekstraksi feature importance untuk analisis faktor risiko.
- **Business Simulation**: Perhitungan potensi penghematan revenue berdasarkan prediksi model.

Kode ini terstruktur secara modular, memungkinkan pengembang lain untuk memodifikasi atau memperluas fungsi tertentu sesuai kebutuhan.