# Prediksi Penyakit Gagal Jantung - Rizky Aditya
Proyek ini dibuat sebagai bahan latihan dalam kursus Machine Learning Terapan dari Dicoding

## Domain Proyek
### Latar Belakang
Penyakit Kardiovaskular (CVD) merupakan penyebab utama kematian di Asia [1] dan juga merupakan penyebab utama kematian di dunia. Penyakit ini menyebabkan
sekitar 17,9 juta kematian setiap tahun, yang menyumbang 31 persen dari seluruh kematian di dunia. Empat dari 5 kematian akibat kardiovaskular disebabkan oleh
serangan jantung dan stroke, dan sepertiga dari kematian tersebut terjadi pada orang dibawah usia pada 70 Tahun. salah satu kejadian umum yang disebabkan oleh
Kardiovaskular adalah Gagal Jantung [2].  

Orang-orang yang mengalami penyakit kardiovaskular membutuhkan deteksi dini untuk mencegah kemungkinan akibat fatal yang disebabkan oleh penyakit ini. Oleh karena itu, diperlukan pengembangan algoritma pembelajaran mesin yang dapat membantu dalam mendeteksi dini penyakit kardiovaskular dan masalah pada jantung.



### Referensi
[1] Zhao, D. (2021). Epidemiological features of cardiovascular disease in Asia. JACC: Asia, 1(1), 1-13.  
[2] https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction

## Business Understanding
Proyek ini melibatkan pemahaman mendalam tentang dampak penyakit kardiovaskular dan gagal jantung terhadap kesehatan masyarakat. Penyakit dengan
tingkat kematian tinggi ini membutuhkan deteksi dini serta pengelolaan yang efektif. Dengan demikian, proyek ini bertujuan untuk menggunakan
pendekatan pembelajaran mesin (Machine Learning) untuk memprediksi kemungkinan terjadinya penyakit gagal jantung berdasarkan data klinis pasien.

### Problem Statement
1. Bagaimana mengidentifikasi faktor-faktor prediksi utama yang berkaitan dengan risiko penyakit gagal jantung?.
2. Bagaimana mengembangkan dan mengevaluasi model pembelajaran mesin untuk memprediksi risiko penyakit gagal jantung?.

### Goals
1. Mengembangkan model prediksi yang dapat mengidentifikasi individu dengan risiko tinggi terkena penyakit gagal jantung.
2. Mengevaluasi kinerja model menggunakan metrik evaluasi yang sesuai untuk memastikan akurasi dan keandalan model.

### Solution Statements
1. Mengimplementasikan algoritma KNN, Logistic Regression dan Decision Tree untuk membangun model prediksi penyakit gagal jantung.
2. Melakukan pemrosesan data yang sesuai, termasuk penskalaan fitur dan penanganan missing value (jika ditemukan).
3. Melakukan pelatihan model menggunakan kedua algoritma dengan menggunakan data yang sudah dipisah menjadi data latih dan data uji.
4. Mengevaluasi kinerja kedua model dengan metrik evaluasi seperti akurasi, presisi, recall, dan f1 score.

## Data Understanding
Proyek ini menggunakan dataset 'Heart Failure Prediction' yang dapat diunduh di [link berikut](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction)
### Berikut Informasi-Informasi yang terdapat dalam dataset :
- Dataset Memiliki Format CSV (Comma-Separated Values).
- Dataset memiliki 918 data observasi dengan 11 Features.
- Tidak ada Missing Values dalam Dataset

### Variabel-Variabel yang terdapat dalam Dataset :
1. **Age** : Usia Pasien Dalam Tahun.
2. **Sex** : Jenis Kelamin Pasien (M : Male/Laki-Laki, F : Female/Perempuan).
3. **ChestPainType** : Jenis Nyeri dada yang dialami pasien (TA : Angina Tipikal, ATA : Angina Atipikal, NAP : Nyeri Dada Non Anginal, ASY : Asimtomatik).
4. **RestingBp** : Tekanan darah istirahat pasien dalam satuan mm Hg (milimeter air raksa)
5. **Cholestrol** : Kolestrol serum pasien dalam satuan mm/dl.
6. **FastingBS** : Kadar gula darah puasa pasien [1: Jika FastingBS>120 mg/dl, 0: sebaliknya].
7. **RestingECG** : Hasil elektrokardiogram istirahat pasien (Normal: Normal, ST: Abnormalitas gelombang ST-T (Inversi gelombang T dan/atau elevasi atau depresi ST > 0.05 mV), LVH: Kemungkinan atau pasti hipertrofi ventrikel kiri menurut kriteria Estes)
8. **MaxHR** : Denyut jantung maksimum yang dicapai oleh pasien (Nilai Numerik antara 60 dan 202)
9. **ExerciseAngina** : Angina yang dipicu oleh latihan (Y : Ya, N : Tidak)
10. **Oldpeak** : Depresi segmen T (Nilai numerik diukur dalam depresi)
11. **ST_Slope** : Kemiringan segmen ST latihan puncak (Up : Naik, Flat : Datar, Down : Turun)
12. **HeartDisease** : Kelas keluaran (1: memiliki penyakit jantung, 0 : Normal)

## Data Preparation

