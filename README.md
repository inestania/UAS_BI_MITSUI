# UAS_BI_MITSUI
UAS KELOMPOK
Inestania Putri Yatman_41823010031
Elfrika Sari M Sinaga_41823010076
Annisa Kamilah Santri_41823010100

# Distribution of Missing Values
  isualisasi Distribution of Missing Values bertujuan untuk memberikan gambaran awal mengenai tingkat dan pola nilai hilang (missing values) pada dataset Mitsui Commodity Prediction Challenge. Histogram ini menunjukkan distribusi rasio nilai hilang pada setiap fitur yang terdapat dalam data pelatihan (train.csv).

Pada grafik, sumbu horizontal merepresentasikan rasio missing values, yaitu proporsi data yang hilang pada masing-masing fitur, sedangkan sumbu vertikal menunjukkan jumlah fitur yang berada pada rentang rasio tersebut. Hasil visualisasi memperlihatkan bahwa sebagian besar fitur memiliki rasio missing values yang sangat rendah atau mendekati nol. Kondisi ini menunjukkan bahwa secara umum kualitas data tergolong baik dan mayoritas variabel memiliki tingkat kelengkapan yang tinggi.

Meskipun demikian, terdapat beberapa fitur dengan rasio missing values yang relatif tinggi. Keberadaan fitur-fitur tersebut perlu mendapatkan perhatian khusus karena nilai hilang dalam jumlah besar berpotensi memengaruhi akurasi dan stabilitas model prediksi. Dalam konteks pemodelan time series dan machine learning, fitur dengan tingkat missing values yang tinggi dapat menyebabkan bias atau penurunan performa jika tidak ditangani dengan tepat.

Oleh karena itu, analisis ini menjadi dasar dalam menentukan strategi penanganan data hilang, seperti melakukan imputasi menggunakan nilai statistik tertentu atau mempertimbangkan untuk mengecualikan fitur dengan tingkat missing values yang ekstrem. Secara keseluruhan, visualisasi ini berperan penting dalam tahap Exploratory Data Analysis (EDA) untuk memahami kualitas dan karakteristik dataset pasar keuangan global yang digunakan dalam tantangan prediksi komoditas Mitsui.
<img width="806" height="316" alt="image" src="https://github.com/user-attachments/assets/cefc1666-ad02-4b2c-ab3f-7b6a8ec5660b" />

# Time Series Plot of Sample Feature
Visualisasi Time Series Plot of Sample Feature digunakan untuk memahami pola pergerakan nilai suatu fitur terhadap waktu pada dataset Mitsui Commodity Prediction Challenge. Grafik ini menampilkan perubahan nilai dari satu fitur contoh (sample feature) yang diambil dari data pelatihan (train.csv), di mana sumbu horizontal merepresentasikan indeks waktu (time index) dan sumbu vertikal menunjukkan nilai numerik dari fitur tersebut.

Berdasarkan hasil visualisasi, terlihat bahwa nilai fitur mengalami fluktuasi yang cukup signifikan sepanjang periode pengamatan. Pada fase awal, nilai cenderung menunjukkan tren penurunan secara bertahap, yang kemudian diikuti oleh kenaikan tajam hingga mencapai titik puncak tertentu. Setelah mencapai nilai maksimum, pergerakan data menjadi lebih tidak stabil dengan pola naik dan turun yang relatif cepat, mencerminkan tingkat volatilitas yang tinggi.

Pola fluktuatif dan volatilitas yang tinggi tersebut menunjukkan bahwa data memiliki karakteristik deret waktu (time series) yang bersifat non-stasioner, di mana nilai rata-rata dan varians tidak konstan sepanjang waktu. Kondisi ini menjadi aspek penting dalam proses pemodelan, karena analisis dan prediksi data komoditas umumnya memerlukan teknik khusus, seperti transformasi data, normalisasi, atau penerapan model time series dan machine learning yang mampu menangkap pola temporal secara efektif.

Secara keseluruhan, visualisasi ini memberikan pemahaman awal mengenai perilaku temporal dari fitur dalam dataset Mitsui dan berperan sebagai dasar dalam menentukan strategi feature engineering serta pemilihan metode prediksi yang sesuai.
<img width="806" height="316" alt="image" src="https://github.com/user-attachments/assets/d60dfddd-132c-45cd-829c-e076cafca693" />


# Actual vs Prediction
Visualisasi Actual vs Prediction digunakan untuk membandingkan nilai aktual target komoditas dengan nilai hasil prediksi model pada data uji (test set) dalam konteks Mitsui Commodity Prediction Challenge. Pada grafik ini, garis Actual merepresentasikan nilai asli yang terdapat pada dataset, sedangkan garis Prediction menunjukkan nilai estimasi yang dihasilkan oleh model baseline berbasis rolling mean.

Model prediksi dibangun menggunakan metode rata-rata bergerak (moving average) dengan ukuran jendela (window size) sebesar lima periode. Pendekatan ini memanfaatkan informasi historis jangka pendek untuk menghasilkan prediksi yang lebih stabil serta mengurangi pengaruh fluktuasi ekstrem pada data. Dataset dibagi secara temporal dengan proporsi 80% sebagai data latih dan 20% sebagai data uji, sehingga evaluasi model dilakukan pada periode waktu yang belum pernah digunakan dalam proses pembentukan prediksi.

Berdasarkan hasil visualisasi, terlihat bahwa kurva prediksi mampu mengikuti pola umum pergerakan nilai aktual, terutama pada tren kenaikan dan penurunan yang terjadi secara bertahap. Namun, pada titik-titik tertentu yang menunjukkan perubahan nilai secara tajam, hasil prediksi cenderung lebih halus dan mengalami keterlambatan (lag) dibandingkan nilai aktual. Kondisi ini merupakan karakteristik umum dari metode moving average yang lebih menekankan kestabilan daripada respons cepat terhadap perubahan mendadak.

Secara keseluruhan, visualisasi ini menunjukkan bahwa model baseline yang digunakan telah mampu menangkap tren utama pada data deret waktu komoditas, meskipun masih memiliki keterbatasan dalam memodelkan volatilitas yang tinggi. Oleh karena itu, hasil ini dapat dijadikan sebagai acuan awal sebelum menerapkan pendekatan pemodelan yang lebih kompleks, seperti model machine learning berbasis lag features atau metode deep learning, guna meningkatkan akurasi prediksi.
<img width="806" height="316" alt="image" src="https://github.com/user-attachments/assets/228a362f-7e4b-4fd2-a3a3-9a8252bb751f" />



