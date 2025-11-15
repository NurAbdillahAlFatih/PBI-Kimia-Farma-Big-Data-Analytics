Kimia Farma Big Data Analytics

Repository ini berisi rangkaian analisis penjualan Kimia Farma periode 2020–2023 menggunakan BigQuery sebagai data warehouse dan Looker Studio sebagai dashboard utama. Proyek difokuskan pada integrasi data transaksi, produk, dan cabang untuk menghasilkan insight operasional yang mendukung pengambilan keputusan bisnis.

📌 Ringkasan Proyek

Analisis dilakukan terhadap lebih dari 600 ribu transaksi. Ruang lingkup mencakup:

pembersihan dan standarisasi data

transformasi dan join tabel

perhitungan metrik (net sales, net profit, discount, rating)

analisis performa provinsi dan tren antar tahun

evaluasi kontribusi kategori produk

Hasil analisis menunjukkan pergeseran pola penjualan antarprovinsi serta penurunan performa di beberapa wilayah.

📁 Struktur Data

Tabel utama yang digunakan:

kf_final_transaction — transaksi lengkap (net sales, net profit, discount, rating)

kf_product — detail produk dan kategori

kf_kantor_cabang — informasi cabang, provinsi, dan rating layanan

Seluruh tabel telah melalui standarisasi tipe data, parsing tanggal, dan perhitungan metrik tambahan.

⚙️ Proses Teknis

Import dataset CSV ke BigQuery

Data cleaning (duplicate removal, normalisasi kolom, validasi ID)

Join transaksi–produk–cabang

Aggregasi berdasarkan provinsi, kategori, dan tahun

Pembuatan dashboard untuk memantau tren penjualan, profit, transaksi, dan performa wilayah

Query SQL dan pipeline transform disertakan dalam repository.

🔍 Temuan Utama

Penjualan 2023 turun tipis dibanding 2022 meskipun rating cabang tetap stabil.

Jawa Barat konsisten menjadi kontributor penjualan terbesar secara nasional.

Empat provinsi mengalami penurunan signifikan: Jawa Timur, Sulawesi Utara, NTB, Kalimantan Timur, yang menjadi penyumbang utama penurunan nasional.

Komposisi kontribusi kategori produk relatif stabil tanpa perubahan besar.

📈 Estimasi Dampak

Penurunan penjualan nasional 2023 terutama berasal dari empat provinsi tersebut.
Berdasarkan share penjualan masing-masing wilayah, potensi pemulihan jika kembali ke level 2022 diperkirakan berada pada rentang:

≈ 0.7% – 0.8% total sales nasional
🧭 Rekomendasi

Tingkatkan kualitas layanan pada cabang yang memiliki gap antara rating cabang dan rating transaksi.

Perkuat strategi pemasaran di provinsi yang mencatat penurunan YoY.

Optimalkan kategori produk yang stagnan melalui bundling, promo terarah, dan penyesuaian stok per wilayah.

Gunakan dashboard operasional untuk monitoring rutin terhadap stock, profit, dan kualitas layanan.
