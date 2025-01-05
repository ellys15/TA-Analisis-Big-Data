# Spotify Songs Data
[image]

# Table of Content
1. [Introduction](#introduction)
2. [Problem](#problem)
3. [Problem Solving Plan](#problem-solving-plan)
4. [Analysis Techniques](#analysis-techniques)
5. [Workflow](#workflow)
6. [Dataset](#dataset)
7. [Dependencies](#dependencies)
8. [Get Started](#get-started)
9. [License](#license)
10. [Team](#team)


## Introduction
Proyek ini berfokus pada analisis data lagu di Spotify untuk mengidentifikasi pola dan faktor utama yang memengaruhi popularitas lagu. Dengan memanfaatkan berbagai teknik seperti Exploratory Data Analysis (EDA), pembersihan data, dan penerapan algoritma pembelajaran mesin, proyek ini bertujuan memberikan wawasan kepada konsumen untuk membuat keputusan yang lebih baik terkait playlist dan rekomendasi musik. Selain itu, proyek ini juga bertujuan memprediksi popularitas lagu sehingga konsumen dapat mengantisipasi lagu baru yang berpotensi menjadi hits. Proyek ini dilaksanakan oleh dua mahasiswa Universitas Muhammadiyah Malang dalam rangka memenuhi tugas mata kuliah Analisis Big Data. Berikut adalah informasi anggota tim:

1. Rania (202110370311)
2. Ellys Rahma Putri Bintoro (202110370311468)


## Problem
Dalam dunia industri musik digital, salah satu tantangan utama yang dihadapi oleh artis, produser, dan pengelola platform musik adalah memahami faktor-faktor yang memengaruhi popularitas sebuah lagu di platform seperti Spotify. Popularitas lagu memiliki dampak signifikan terhadap kesuksesan musisi dan strategi distribusi musik, sehingga analisis pola dan tren musik menjadi langkah penting untuk meningkatkan daya tarik lagu di pasar serta menciptakan pengalaman mendengarkan yang optimal bagi pengguna.

Dengan menggunakan Spotify Songs Dataset, analisis dapat dilakukan untuk menggali wawasan tentang pola-pola yang memengaruhi popularitas lagu. Dataset ini memberikan peluang bagi penggunanya untuk memahami tren musik dan membantu dalam mengambil keputusan berbasis data yang lebih baik.


## Problem Solving Plan
[image]

Data yang tersedia meliputi informasi mengenai nama playlist, id playlist, genre, tempo, instrumental, energi lagu, dan masih banyak lagi. Analisis ini akan dilakukan menggunakan metodologi yang terdiri dari beberapa tahapan, yaitu:

1. Pra-pemrosesan Data: Mengatasi nilai yang hilang, serta normalisasi atau standarisasi fitur numerik yang relevan untuk analisis lebih lanjut.
2. Pemodelan: Menggunakan teknik pembelajaran mesin, seperti Random Forest Classifier atau Random Forest Regressor, untuk memprediksi popularitas lagu berdasarkan fitur yang ada. Dengan model ini, kita dapat menentukan apakah atribut musik tertentu memiliki pengaruh besar terhadap popularitas lagu.
3. Evaluasi Model: Menggunakan metrik evaluasi seperti akurasi, precision, recall, F1-score untuk menilai kinerja model dalam memprediksi kategori popularitas lagu (misalnya: "Populer" dan "Tidak Populer"). Selain itu, visualisasi seperti confusion matrix akan digunakan untuk memahami performa prediksi model.


## Analysis Techniques
[image]

Pada tahap awal, dilakukan proses eksplorasi data (EDA) untuk menganalisis distribusi dan pola yang terdapat dalam dataset. Berbagai teknik visualisasi, seperti grafik distribusi, histogram, dan heatmap, digunakan untuk mengenali variabel-variabel yang berpotensi memengaruhi popularitas lagu secara signifikan. Selain itu, EDA juga berfungsi untuk mengidentifikasi keberadaan data yang hilang atau outlier, yang perlu ditangani guna meningkatkan akurasi model yang akan dibangun.

Analisis ini berfokus pada penerapan pemodelan klasifikasi untuk memprediksi tingkat popularitas lagu (populer atau tidak populer). Algoritma Random Forest digunakan karena kemampuannya dalam mengungkap variabel-variabel kunci yang memengaruhi popularitas lagu serta memprediksi peluang sebuah lagu untuk menjadi populer di masa depan. Algoritma ini memiliki keunggulan dalam mengatasi overfitting, terutama pada dataset yang memiliki banyak fitur, sekaligus memberikan wawasan berharga melalui analisis feature importance yang dihasilkan oleh model.


## Workflow
[image]

Proses analisis diawali dengan mengimpor berbagai package yang diperlukan, seperti [Pandas](https://pandas.pydata.org/) untuk pengolahan data, [NumPy](https://numpy.org/) untuk operasi numerik dan array [Matplotlib](https://matplotlib.org/) dan [Seaborn](https://seaborn.pydata.org/) untuk keperluan visualisasi, serta [scikit-learn](https://scikit-learn.org/stable/) untuk normalisasi, encoding, pemodelan dan evaluasi. Setelah itu, dataset diimpor untuk memulai analisis.

Setelah dataset dimuat, tahap pertama adalah Exploratory Data Analysis (EDA), di mana data dieksplorasi untuk memahami distribusi variabel, hubungan antar fitur, dan mendeteksi masalah seperti data yang hilang atau pencilan.

Kemudian, proses Preprocessing dilakukan untuk menyiapkan data agar siap digunakan dalam model pembelajaran mesin. Langkah ini meliputi penanganan data yang hilang, konversi variabel kategorikal menjadi format numerik, dan normalisasi data.

Setelah data siap, tahap Modeling dimulai, pada kasus ini model yang digunakan adalah [Random Forest](https://scikit-learn.org/1.5/modules/generated/sklearn.ensemble.RandomForestClassifier.html). Diterapkan untuk memprediksi pemesanan dan pembatalan berdasarkan fitur yang tersedia.

Terakhir, Evaluation dilakukan untuk menilai kinerja model menggunakan [evaluation metrics]([https://scikit-learn.org/1.5/api/sklearn.metrics.html](https://scikit-learn.org/stable/api/sklearn.metrics.html)) seperti akurasi, precision, recall, dan F1-score, guna memastikan model dapat memprediksi dengan baik dan akurat.


## Dataset
Dataset yang digunakan diambil dari github [Penjelasan Data](https://github.com/rfordatascience/tidytuesday/blob/main/data/2020/2020-01-21/readme.md). Dataset ini berisi informasi mengenai _track_id, track_name, track_artist, track_popularity, playlist_name, playlist_id, playlist_genre, tempo, instrumental_, dan masih banyak variabel lainnya lagi yang tentunya dengan class/tipe data yang berbeda. Tipe data/claass yang tersedia pada dataset ini adalah integer, float, dan object. Dataset dapat di download [disini]([https://github.com/rfordatascience/tidytuesday/blob/main/data/2020/2020-02-11/hotels.csv](https://www.dropbox.com/sh/qj0ueimxot3ltbf/AACzMOHv7sZCJsj3ErjtOG7ya?dl=1))


## Dependencies
Berikut daftar dependensi yang dibutuhkan agar code yang tertera dapar dijalankan dengan baik :
1. pandas
2. numpy
3. matplotlib
4. seaborn
5. scikit-learn

## Get Started
Untuk memulai proyek ini, pastikan Anda telah menginstal semua package yang dibutuhkan. Anda dapat melakukannya dengan mengikuti langkah-langkah berikut:

1. **Clone repository** ini ke mesin lokal Anda:
   ```bash
   git clone https://github.com/ellys15-TA-Analisis-Big-Data.git
   ```

2. **Instal dependencies** menggunakan `pip`:
   ```bash
   pip install -r requirements.txt
   ```

3. **Impor dataset**: Pastikan Anda memiliki [dataset]([https://github.com/rfordatascience/tidytuesday/blob/main/data/2020/2020-02-11/hotels.csv](https://www.dropbox.com/sh/qj0ueimxot3ltbf/AACzMOHv7sZCJsj3ErjtOG7ya?dl=1)) yang sesuai dan letakkan di direktori yang telah ditentukan dalam kode.

4. **Jalankan Kode**: Jalankan kode sesuai dengan urutan yang sudah ada.

## License
Repository ini dibuat dengan akses penuh.

## Team
- [Rania](https://github.com/Septiannisa13)
- [Ellys Rahma Putri Bintoro](https://github.com/ellys15)
