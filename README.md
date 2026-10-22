# Analisis-Pola-Pembelian-Konsumen-Apriori-vs-FP-Growth
Market Basket Analysis menggunakan Frequent Pattern Mining untuk menemukan hubungan antarproduk dan menghasilkan insight bisnis pada sektor retail.

## Tentang Proyek

Proyek ini bertujuan untuk menganalisis pola pembelian konsumen berdasarkan data transaksi retail menggunakan dua algoritma data mining, yaitu Apriori dan FP-Growth. Analisis dilakukan untuk menemukan kombinasi produk yang sering dibeli secara bersamaan (frequent itemsets) serta hubungan antarproduk melalui association rules.

Selain menemukan pola pembelian, proyek ini juga membandingkan performa kedua algoritma berdasarkan jumlah pola yang ditemukan, kualitas aturan asosiasi, dan waktu komputasi. Hasil analisis kemudian diinterpretasikan menjadi insight bisnis yang dapat mendukung strategi pemasaran retail berbasis data.

## Tujuan Proyek
Mengidentifikasi produk yang sering dibeli oleh konsumen.

Menemukan hubungan antarproduk menggunakan association rule mining.

Membandingkan performa algoritma Apriori dan FP-Growth.

Menghasilkan insight untuk strategi product bundling, cross-selling, dan product placement.


📂 Dataset

Dataset yang digunakan adalah Retail Market Basket Transactions dari Kaggle.

Jumlah transaksi: 7.501

Jumlah item unik: 119

Jumlah kolom item awal: 20

Sumber dataset: Retail Market Basket Transactions – Kaggle

⚙️ Metodologi

Exploratory Data Analysis (EDA) — memahami struktur dataset, frekuensi produk, distribusi jumlah item per transaksi, dan outlier.

Data Preprocessing — membersihkan nama produk, menangani missing values, memeriksa transaksi duplikat, dan membentuk daftar transaksi.

Data Transformation — mengubah data transaksi menjadi matriks biner menggunakan one-hot encoding.

Frequent Pattern Mining — menerapkan algoritma Apriori dan FP-Growth untuk menemukan kombinasi produk yang sering muncul.

Association Rule Mining — membentuk aturan asosiasi berdasarkan support, confidence, dan lift.

Evaluasi dan Perbandingan — membandingkan jumlah frequent itemsets, association rules, metrik asosiasi, serta runtime kedua algoritma.

Business Insight — menginterpretasikan pola yang ditemukan menjadi rekomendasi strategi bisnis retail.

🧰 Tools & Technologies

Python — bahasa pemrograman untuk analisis data.

Pandas & NumPy — pengolahan dan manipulasi data.

Matplotlib — visualisasi data dan hasil analisis.

MLxtend — implementasi algoritma Apriori, FP-Growth, dan association rules.

Google Colab / Jupyter Notebook — lingkungan pengembangan dan eksperimen.

📊 Hasil Utama

Dengan minimum support sebesar 0,01 dan minimum confidence sebesar 0,3, diperoleh hasil berikut:

Indikator

Apriori

FP-Growth

Frequent itemsets

257

257

Association rules

63

63

Rata-rata confidence

0,3683

0,3683

Rata-rata lift

1,7742

1,7742

Runtime

0,438 detik

4,670 detik

Pada pengujian ini, kedua algoritma menghasilkan frequent itemsets dan association rules yang sama. Namun, Apriori memiliki waktu komputasi lebih singkat pada dataset yang digunakan.

🔎 Temuan Menarik

Aturan asosiasi dengan nilai lift tertinggi menunjukkan hubungan antara herb & pepper dan ground beef.

Support: 0,0160

Confidence: 0,3235

Lift: 3,2920

Nilai lift yang lebih besar dari 1 menunjukkan bahwa kedua produk memiliki asosiasi positif pada dataset.

💡 Insight Bisnis

Temuan pola pembelian dapat dimanfaatkan untuk:

Product Bundling: menawarkan herb & pepper bersama ground beef sebagai paket produk pelengkap.

Cross-Selling: menawarkan spaghetti kepada konsumen yang membeli ground beef dan mineral water.

Product Placement: mempertimbangkan penempatan olive oil dan spaghetti pada area rak yang berdekatan.

Rekomendasi tersebut merupakan interpretasi berdasarkan pola asosiasi, bukan jaminan bahwa strategi tersebut akan meningkatkan penjualan.

🏆 Kesimpulan

Berdasarkan hasil eksperimen pada dataset ini, Apriori menjadi pilihan yang lebih efisien karena menghasilkan jumlah frequent itemsets dan association rules yang sama dengan FP-Growth, tetapi dengan runtime yang lebih singkat. Hasil penelitian juga menunjukkan bagaimana teknik data mining dapat digunakan untuk mengubah data transaksi menjadi informasi yang mendukung pengambilan keputusan bisnis.

Performa tersebut berlaku pada dataset dan implementasi yang diuji, sehingga belum dapat digeneralisasikan untuk semua dataset retail.

📁 Isi Repository

Code_Hasil_Akhir_Kelompok_8.ipynb — notebook analisis, preprocessing, implementasi algoritma, visualisasi, dan evaluasi.

Laporan Pemaparan Hasil Akhir_kelompok 8.pdf — laporan penelitian yang menjelaskan metodologi, hasil, pembahasan, dan kesimpulan.

👥 Tim Peneliti

Program Studi S1 Sains Data
Universitas Negeri Surabaya (UNESA)
Kelas 2024B

Adisti Eka Nabila

Umi Imro'atus Sholekhah

Maris Al Sabina Azzuhra
