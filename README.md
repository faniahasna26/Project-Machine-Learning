**Deskripsi Projek**

Projek ini bertujuan untuk membangun model *machine learning* yang dapat memprediksi kemungkinan seorang karyawan mengalami **attrition** (keluar dari perusahaan) berdasarkan karakteristik demografi, pekerjaan, dan performa karyawan. Prediksi attrition penting dilakukan karena tingginya tingkat pergantian karyawan dapat meningkatkan biaya rekrutmen, pelatihan, serta menurunkan produktivitas perusahaan. Data yang digunakan dalam penelitian ini merupakan **data sekunder** yang diperoleh dari **dataset IBM HR Analytics Employee Attrition & Performance** yang tersedia secara publik melalui platform Kaggle. Dataset ini memuat berbagai informasi mengenai karyawan, seperti usia, departemen, tingkat pendidikan, pendapatan bulanan, kepuasan kerja, keseimbangan kehidupan kerja (*work-life balance*), lembur (*overtime*), masa kerja, dan berbagai atribut lainnya yang diduga memengaruhi keputusan karyawan untuk tetap bekerja atau mengundurkan diri. Permasalahan dalam proyek ini termasuk ke dalam **klasifikasi biner**, dengan variabel target **Attrition** yang terdiri atas dua kelas, yaitu *Yes* dan *No*. Proses yang dilakukan meliputi eksplorasi data (*Exploratory Data Analysis*), prapemrosesan data, rekayasa fitur, pelatihan dan perbandingan beberapa algoritma klasifikasi, penyetelan *hyperparameter*, serta evaluasi model menggunakan metrik klasifikasi yang sesuai. Hasil dari proyek ini diharapkan mampu memberikan model prediksi yang akurat serta mengidentifikasi faktor-faktor utama yang memengaruhi attrition sehingga dapat menjadi dasar dalam mendukung pengambilan keputusan di bidang manajemen sumber daya manusia.

**Nama Anggota Kelompok**
1. Fania Hasna Rasyida (K1D024001)
2.  Nabila Dwi Setiawati (K1D024005)
3. Kinanti Jingga Adzhani (K1D024007)
4. Amelia Wulandari (K1D024027)
5. Hafdsa Syafiya (K1D024040)

**Sumber Dataset**

Data yang digunakan dalam penelitian ini merupakan data sekunder yang berasal dari dataset IBM HR Analytics Employee Attrition & Performance. Dataset tersebut dipublikasikan melalui platform Kaggle dan berisi data mengenai karakteristik demografi, pekerjaan, serta performa karyawan yang digunakan untuk menganalisis faktor-faktor yang memengaruhi employee attrition. Dataset ini terdiri dari 1.470 observasi dan 35 variabel, dengan variabel target Attrition yang memiliki dua kategori, yaitu Yes dan No. Dataset dapat diakses melalui tautan berikut: https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset

**Cara Menjalankan**
1. Unduh seluruh file proyek dari repository GitHub.
2. Pastikan Python telah terinstal pada perangkat.
3. Instal seluruh library yang dibutuhkan menggunakan perintah:
   pip install -r requirements.txt
4. Buka file notebook (.ipynb) menggunakan Jupyter Notebook atau Google Colab.
5. Pastikan dataset Attrition.csv berada pada folder yang sama dengan notebook atau unggah dataset jika menggunakan Google Colab.
6. Jalankan notebook secara berurutan mulai dari proses pembacaan data, eksplorasi data (EDA), preprocessing, pemodelan, hingga
   evaluasi model.
7. Hasil evaluasi model akan ditampilkan secara otomatis dalam bentuk metrik klasifikasi dan confusion matrix.

**Hasil**

Proyek ini bertujuan membangun model klasifikasi untuk memprediksi Employee Attrition menggunakan dataset IBM HR Analytics Employee Attrition & Performance dari Kaggle. Tahapan yang dilakukan meliputi eksplorasi data, penanganan outlier menggunakan metode IQR, encoding variabel kategorik, normalisasi dan standarisasi data, pembagian data dengan rasio 80:20, serta penyeimbangan kelas menggunakan SMOTE. Selanjutnya dilakukan pemodelan menggunakan tiga algoritma, yaitu Logistic Regression, Random Forest, dan XGBoost.
Hasil evaluasi menunjukkan bahwa Logistic Regression memperoleh nilai recall tertinggi sebesar 81,58%, sehingga mampu mengidentifikasi lebih banyak karyawan yang berpotensi mengalami attrition dibandingkan model lainnya. Meskipun Random Forest memiliki akurasi tertinggi sebesar 87,05%, model tersebut memiliki nilai recall yang lebih rendah sehingga lebih banyak melewatkan kasus attrition. Oleh karena itu, Logistic Regression dipilih sebagai model yang direkomendasikan karena lebih sesuai dengan tujuan bisnis, yaitu membantu perusahaan mengurangi tingkat employee attrition dengan mendeteksi sebanyak mungkin karyawan yang berpotensi keluar sehingga perusahaan dapat mengambil langkah pencegahan berdasarkan faktor-faktor yang memengaruhinya.
