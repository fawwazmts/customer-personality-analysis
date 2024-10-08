# Analisis Kepribadian Pelanggan (Customer Personality Analysis)

## 1. Pendahuluan

### 1.1 Masalah Bisnis

Perusahaan memiliki data pelanggan berisi informasi tentang pelanggan, belanja produk, respon terhadap promosi, dan jumlah pembelian melalui saluran pembelian yang ada. Perusahaan ingin memahami kepribadian dan perilaku pelanggan untuk mengembangkan strategi pemasaran yang lebih personal dan efektif, serta meningkatkan loyalitas pelanggan dan penjualan.

### 1.2 Pertanyaan Bisnis

1. Bagaimana karakteristik pelanggan yang paling banyak melakukan pembelian produk dalam 2 tahun terakhir?
2. Bagaimana hubungan antara pendapatan tahunan rumah tangga dan total pengeluaran untuk belanja dalam 2 tahun terakhir?
3. Bagaimana produk yang dibeli berdasarkan karakteristik pelanggan?
4. Bagaimana efektivitas kampanye promosi yang ada saat ini?
5. Apa saluran pembelian (web, katalog, toko) yang paling banyak digunakan oleh pelanggan?
6. Apa karakteristik pelanggan yang melakukan pembelian melalui saluran pembelian?

## 2. Deskripsi Data

### 2.1 Sumber Data

Data yang digunakan pada analisis ini dapat diakses [di sini](https://github.com/fawwazmts/customer-personality-analysis/blob/main/Supermarket%20Customers.csv).

### 2.2 Kamus Data Pelanggan Supermarket

1. **Informasi Pelanggan**

   * **ID**: Identifikasi unik pelanggan
   * **Year_Birth**: Tahun lahir pelanggan
   * **Education**: Tingkat pendidikan pelanggan
   * **Marital_Status**: Status pernikahan pelanggan
   * **Income**: Pendapatan tahunan rumah tangga pelanggan
   * **Kidhome**: Jumlah anak di rumah tangga pelanggan
   * **Teenhome**: Jumlah remaja di rumah tangga pelanggan
   * **Dt_Customer**: Tanggal pendaftaran pelanggan di perusahaan
   * **Recency**: Jumlah hari sejak pembelian terakhir pelanggan
   * **Complain**: 1 jika pelanggan menyampaikan keluhan dalam 2 tahun terakhir, 0 sebaliknya
2. **Belanja Produk**

   * **MntWines**: Jumlah yang dibelanjakan untuk anggur dalam 2 tahun terakhir
   * **MntFruits**: Jumlah yang dibelanjakan untuk buah dalam 2 tahun terakhir
   * **MntMeatProducts**: Jumlah yang dibelanjakan untuk daging dalam 2 tahun terakhir
   * **MntFishProducts**: Jumlah yang dibelanjakan untuk ikan dalam 2 tahun terakhir
   * **MntSweetProducts**: Jumlah yang dibelanjakan untuk makanan manis dalam 2 tahun terakhir
   * **MntGoldProds**: Jumlah yang dibelanjakan untuk emas dalam 2 tahun terakhir
3. **Respon terhadap Promosi**

   * **NumDealsPurchases**: Jumlah pembelian dengan diskon
   * **AcceptedCmp1**: 1 jika pelanggan menerima tawaran pada kampanye ke-1, 0 sebaliknya
   * **AcceptedCmp2**: 1 jika pelanggan menerima tawaran pada kampanye ke-2, 0 sebaliknya
   * **AcceptedCmp3**: 1 jika pelanggan menerima tawaran pada kampanye ke-3, 0 sebaliknya
   * **AcceptedCmp4**: 1 jika pelanggan menerima tawaran pada kampanye ke-4, 0 sebaliknya
   * **AcceptedCmp5**: 1 jika pelanggan menerima tawaran pada kampanye ke-5, 0 sebaliknya
   * **Response**: 1 jika pelanggan menerima tawaran pada kampanye terakhir, 0 sebaliknya
4. **Saluran Pembelian**

   * **NumWebPurchases**: Jumlah pembelian yang dilakukan melalui situs web perusahaan
   * **NumCatalogPurchases**: Jumlah pembelian yang dilakukan menggunakan katalog
   * **NumStorePurchases**: Jumlah pembelian yang dilakukan langsung di toko
   * **NumWebVisitsMonth**: Jumlah kunjungan ke situs web perusahaan dalam sebulan terakhir
5. **Kolom Lain**

   * **Z_CostContact**: Kolom yang tidak relevan dengan data
   * **Z_Revenue**: Kolom yang tidak relevan dengan data

### 2.3 Langkah-langkah Analisis

Langkah lengkap terkait Analisis Kepribadian Pelanggan (Customer Personality Analysis) dapat diakses [di sini](https://github.com/fawwazmts/customer-personality-analysis/blob/main/CustomerPersonalityAnalysis.ipynb).

Secara umum, berikut merupakan langkah analisis data pada projek ini.

1. Introduction

   * Definisikan business problem
   * Definisikan business question
2. Data Preparation

   1. Data Understanding

      * Memahami deskripsi dataset
      * Memahami informasi pada data secara umum
      * Memahami informasi pada data secara spesifik (per kolom)
      * Mengidentifikasi format dan tipe data, data yang hilang, anomali nilai pada data, dan kolom yang tidak relevan untul ditangani pada Data Cleaning
   2. Data Cleaning

      * Penanganan format dan tipe data
      * Penanganan data yang hilang
      * Penanganan data pencilan
      * Penanganan anomali nilai pada data
      * Penanganan kolom yang tidak relevan
      * Penambahan kolom baru sesuai kebutuhan analisis
   3. Data Analysis

      * Analisis data untuk menjawab business question yang telah didefinisikan
   4. Conclusion and Recommendation

      * Conclusion
      * Recommendation

## 3. Simpulan dan Rekomendasi

### 3.1 Simpulan

- Pelanggan yang paling banyak melakukan pembelian dalam 2 tahum terakhir adalah kelompok pelanggan Adult (36-55 tahun), Bachelor's, Maried, dan tidak memili anak di rumah.
- Pelanggan yang paling sedikit melakukan pembelian dalam 2 tahum terakhir adalah kelompok pelanggan Young Adult (19-35 tahun), Basic, Widow, dan memiliki 3 anak.
- Produk yang dengan pembelian paling banyak adalah Anggur, setelah itu daging.
- Produk yang dengan pembelian paling sedikit adalah buah, ikan, makanan manis, dan emas. Pembelian emas termasuk sedikt mungkin karena emas termasuk barang untuk investasi dan pembelian tidak teratur dalam jumlah banyak. Pembelian buah, ikan, dan makanan termasuk sedikit mungkin karena barang tersebut kurang diminati.
- Semua kategori pelanggan, baik berdasarkan kelompok umur, tingkat pendidikan, status pernikahan, dan total anak di rumah, melakukan pembelian paling banyak pada produk anggur.
- Kampanye promosi yang dilakukan terindikasi tidak efektik. Mayoritas pelanggan sama sekali tidak pernah menerima penawaran kampanye.
- Pelanggan paling banyak melakukan pembelian melalui toko dan paling sedikit melakukan pembelian melalui katalog.
- Karakteristik pelanggan yang paling banyak melakukan pembelian melalui toko dan web mirip, yaitu Adult, Bachelor's, Maried, dan memiliki 1 anak.
- Karakteristik pelanggan yang paling banyak melakukan pembelian melalui katalog hanya berbeda pada jumlah anak yang dimiliki pelanggan, yaitu tidak memimiliki anak.
- Karakteristik pelanggan yang paling sedikit melakukan pembelian di web, katalog, dan toko mirip, yaitu Young Adult, Basic, Widow, dan memiliki 3 anak.

### 3.2 Rekomendasi

- Kampanye promosi perlu diperbaiki agar lebih efektif dengan cara menyasar pelanggan yang tepat dengan promo yang tepat.
- Jika perusahaan ingin meningkatkan loyalitas, memperkuat hubungan, dan menjaga kepuasan pelanggan untuk memastikan pelanggan terus melakukan pembelian, maka maka promo dapat difokuskan pada pelanggan yang paling banyak melakukan pembelian dalam 2 tahum terakhir, yaitu Adult (36-55 tahun), Bachelor's, Maried, dan tidak memili anak di rumah. Promo yang dapat diterapkan dapat berupa diskon besar atau penawaran khusus yang hanya tersedia untuk pelanggan yang paling banyak melakukan pembelian, hadiah loyalitas, dan layanan prioritas. Selain itu, fokus promo ini juga dapat diterapkan pada produk dengan pembelian paling banyak seperti anggur dan daging.
- Jika perusahaan ingin meningkatkan frekuensi pembelian, mengonversi pelanggan yang lebih aktif, dan meningkatkan nilai pembelian rata-rata, maka promo dapat difokuskan pada pelanggan yang paling sedikit melakukan pembelian dalam 2 tahum terakhir, yaitu kelompok pelanggan Young Adult (19-35 tahun), Basic, Widow, dan memiliki 3 anak. Promo fokus pada insentif untuk memotivasi pembelian tambahan. Promo yang dapat diterapkan dapat berupa diskon besar untuk pembelian pertama atau kedua untuk mendorong percobaan produk, paket bundling dengan produk tambahan untuk mendorong pembelian lebih banyak, menawarkan diskon atau hadiah jika mereka merekomendasikan produk kepada orang lain, dan memberikan poin loyalitas untuk setiap pembelian dengan tujuan meningkatkan frekuensi pembelian. Selain itu, fokus promo ini juga dapat diterapkan pada produk dengan pembelian paling sedikit seperti buah, ikan, makanan manis, dan emas.
- Pada saluran pembelian yang paling banyak digunakan pelanggan seperti toko, perusaahaan dapat melakukan promo dengan fokus memaksimalkan penjualan, memanfaatkan volume lalu lintas tinggi, dan meningkatkan konversi. Promo yang dapat dilakukan diantaranya, diskon besar atau penawaran menarik untuk meningkatkan penjualan, seperti diskon volume atau penawaran beli 1 gratis 1, penawaran atau produk eksklusif untuk pelanggan di saluran tersebut, dan promosi untuk meningkatkan nilai pembelian dengan menawarkan produk tambahan yang relevan.
- Pada saluran pembelian yang paling sedikit digunakan pelanggan seperti katalog, perusaahaan dapat melakukan promo dengan fokus meningkatkan kunjungan dan visibilitas, mendorong penggunaan saluran, dan mengubah saluran menjadi lebih aktif. Promo yang dapat dilakukan diantaranya, diskon besar atau penawaran khusus untuk menarik pelanggan baru ke saluran tersebut, menggabungkan produk dengan harga khusus atau bundling yang menarik untuk memotivasi pembelian, penawaran waktu terbatas untuk menciptakan rasa urgensi dan mendorong kunjungan ke saluran tersebut.


## Catatan Tambahan

Dashboard yang berkaitan dengan analisis ini dapat diakses [di sini](https://public.tableau.com/views/CustomerPersonalityAnalysis_17247480326150/DashboardCPA?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link). Dashboard ini dibuat menggunakan Tableau.
