# Analisis-Pola-Pembelian-Konsumen-Apriori-vs-FP-Growth
Market Basket Analysis menggunakan Frequent Pattern Mining untuk menemukan hubungan antarproduk dan menghasilkan insight bisnis pada sektor retail.

## Tentang Proyek

Proyek ini bertujuan untuk menganalisis pola pembelian konsumen berdasarkan data transaksi retail menggunakan dua algoritma data mining, yaitu Apriori dan FP-Growth. Analisis dilakukan untuk menemukan kombinasi produk yang sering dibeli secara bersamaan (frequent itemsets) serta hubungan antarproduk melalui association rules.

Selain menemukan pola pembelian, proyek ini juga membandingkan performa kedua algoritma berdasarkan jumlah pola yang ditemukan, kualitas aturan asosiasi, dan waktu komputasi. Hasil analisis kemudian diinterpretasikan menjadi insight bisnis yang dapat mendukung strategi pemasaran retail berbasis data.

## Tujuan Proyek
1. Mengidentifikasi produk yang sering dibeli oleh konsumen.
2. Menemukan hubungan antarproduk menggunakan association rule mining.
3. Membandingkan performa algoritma Apriori dan FP-Growth.
4. Menghasilkan insight untuk strategi product bundling, cross-selling, dan product placement.


## 📂 Dataset
Dataset yang digunakan adalah Retail Market Basket Transactions dari Kaggle.
Jumlah transaksi: 7.501
Jumlah item unik: 119
Jumlah kolom item awal: 20
Sumber dataset: Retail Market Basket Transactions – Kaggle

## 🧰 Tools & Technologies
Python — bahasa pemrograman untuk analisis data.
Pandas & NumPy — pengolahan dan manipulasi data.
Matplotlib — visualisasi data dan hasil analisis.
MLxtend — implementasi algoritma Apriori, FP-Growth, dan association rules.
Google Colab / Jupyter Notebook — lingkungan pengembangan dan eksperimen.

## 📊 Hasil Utama

Dengan minimum support sebesar 0,01 dan minimum confidence sebesar 0,3, diperoleh hasil berikut:

| Indikator | Apriori | FP-Growth |
|---|---:|---:|
| Frequent itemsets | 257 | 257 |
| Association rules | 63 | 63 |
| Rata-rata confidence | 0,3683 | 0,3683 |
| Rata-rata lift | 1,7742 | 1,7742 |
| Runtime | 0,438 detik | 4,670 detik |
Pada pengujian ini, kedua algoritma menghasilkan frequent itemsets dan association rules yang sama. Namun, Apriori memiliki waktu komputasi lebih singkat pada dataset yang digunakan.

## 💡 Insight Bisnis
Temuan pola pembelian dapat dimanfaatkan untuk:
1. Product Bundling: menawarkan herb & pepper bersama ground beef sebagai paket produk pelengkap.
2. Cross-Selling: menawarkan spaghetti kepada konsumen yang membeli ground beef dan mineral water.
3. Product Placement: mempertimbangkan penempatan olive oil dan spaghetti pada area rak yang berdekatan.

Rekomendasi tersebut merupakan interpretasi berdasarkan pola asosiasi, bukan jaminan bahwa strategi tersebut akan meningkatkan penjualan.

## 🏆 Kesimpulan

Berdasarkan hasil eksperimen pada dataset ini, Apriori menjadi pilihan yang lebih efisien karena menghasilkan jumlah frequent itemsets dan association rules yang sama dengan FP-Growth, tetapi dengan runtime yang lebih singkat. Hasil penelitian juga menunjukkan bagaimana teknik data mining dapat digunakan untuk mengubah data transaksi menjadi informasi yang mendukung pengambilan keputusan bisnis.

Performa tersebut berlaku pada dataset dan implementasi yang diuji, sehingga belum dapat digeneralisasikan untuk semua dataset retail.

## Tim Peneliti
Adisti Eka Nabila
Umi Imro'atus Sholekhah
Maris Al Sabina Azzuhra
