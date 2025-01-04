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


