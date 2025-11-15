Kimia Farma Big Data Analytics

Repository ini memuat rangkaian analisis penjualan Kimia Farma periode 2020–2023 menggunakan BigQuery sebagai data warehouse dan Looker Studio sebagai dashboard utama. Proyek ini berfokus pada integrasi data transaksi, produk, dan cabang untuk menghasilkan insight operasional yang dapat digunakan dalam pengambilan keputusan bisnis.

Ringkasan Proyek

Analisis dilakukan terhadap lebih dari 600 ribu data transaksi. Proses mencakup pembersihan data, transformasi, perhitungan metrik penjualan, serta pembuatan visualisasi. Hasil analisis menunjukkan perubahan pola penjualan antarprovinsi, identifikasi penurunan performa di wilayah tertentu, serta evaluasi kontribusi kategori produk.

Struktur Data

Tabel utama yang digunakan:

kf_final_transaction: transaksi lengkap dengan net sales, net profit, discount, dan rating.

kf_product: detail produk dan kategori.

kf_kantor_cabang: informasi cabang, provinsi, dan rating layanan.

Semua tabel telah melalui standarisasi tipe data, parsing tanggal, serta perhitungan metrik tambahan seperti net sales dan net profit.

Proses Teknis

Import CSV ke BigQuery.

Data cleaning (duplicate removal, normalisasi kolom, validasi ID).

Join tabel transaksi–produk–cabang.

Aggregasi berdasarkan provinsi, kategori, dan tahun.

Pembuatan dashboard untuk tren penjualan, profit, transaksi, dan performa wilayah.

Query SQL dan pipeline transform tersedia di repository ini.

Temuan Utama

Penjualan 2023 mengalami penurunan kecil meski rating cabang tetap stabil.

Jawa Barat konsisten menjadi kontributor terbesar secara nasional.

Empat provinsi menunjukkan penurunan signifikan (Jawa Timur, Sulawesi Utara, NTB, Kalimantan Timur) dan menjadi sumber utama penurunan total nasional.

Kontribusi kategori produk relatif stabil tanpa perubahan besar.

Estimasi Dampak

Penurunan penjualan nasional 2023 sebagian besar berasal dari empat provinsi tersebut. Berdasarkan share penjualan masing-masing wilayah, potensi pemulihan diperkirakan sekitar 0.7–0.8% apabila performanya kembali ke level tahun sebelumnya.

Rekomendasi

Fokus peningkatan layanan untuk cabang dengan gap antara rating cabang dan rating transaksi.

Percepatan strategi pemasaran di provinsi yang mengalami penurunan YoY.

Optimalisasi kategori produk yang stagnan melalui bundling dan penyesuaian promo per wilayah.

Pemanfaatan dashboard operasional untuk monitoring rutin stock, profit, dan kualitas layanan.
