# ☕ Kedai Ngopi-Lah - Digital Coffee Shop & Order System

Website platform digital komprehensif untuk manajemen dan pemesanan menu kafe secara *real-time*. Proyek ini menggabungkan antarmuka statis yang interaktif dengan sistem pemrosesan transaksi serta manajemen data dinamis di sisi server.

🔗 **Live Website**: [kedai-ngopi-lah.vercel.app](https://vercel.app)

---

## 📌 Daftar Isi
1. [Fitur Utama](#-fitur-utama)
2. [Teknologi & Komposisi Kode](#-teknologi--komposisi-kode)
3. [Arsitektur Folder Proyek](#-arsitektur-folder-proyek)
4. [Alur & Mekanisme Sistem Backend](#-alur--mekanisme-sistem-backend)
5. [Instalasi & Pengoperasian Lokal](#-instalasi--pengoperasian-lokal)

---

## 🚀 Fitur Utama

* **🛒 Interactive Shopping Cart**: Tamu dapat memilih varian kopi, mengatur jumlah pesanan, dan melihat total biaya belanja secara instan tanpa perlu memuat ulang halaman.
* **📋 Dynamic Menu Display**: Katalog menu kopi dan camilan yang tertata rapi, lengkap dengan harga, deskripsi produk, dan gambar visual yang menggugah selera.
* **💼 Backend Transaction Handler**: Pemrosesan formulir pesanan, validasi transaksi, dan pencatatan data pembelian di sisi server secara aman.
* **📱 Responsive Layout**: Antarmuka berbasis *mobile-first design* yang sangat nyaman diakses dari smartphone pelanggan saat berada di meja kafe.

---

## 🛠️ Teknologi & Komposisi Kode

Proyek ini menggunakan arsitektur *full-stack* ringan dengan dominasi proses pada sektor *back-end engine*:

* **PHP** (74.0%) - Menangani logika bisnis backend, pemrosesan transaksi, manajemen menu, dan sesi pelanggan.
* **HTML5** (12.4%) - Kerangka semantik untuk menyusun tata letak halaman utama kafe.
* **CSS3** (8.7%) - Desain visual kustom, animasi transisi, dan penataan gaya estetik bertema kafe modern.
* **JavaScript** (4.9%) - Mengatur interaktivitas mikro, kalkulasi dinamis pada keranjang belanja, dan pembaruan UI klien.

---

## 📂 Arsitektur Folder Proyek

Berikut adalah pemetaan berkas utama untuk memudahkan navigasi pengembangan komponen:

```text
kedai-ngopi-lah/
│
├── src/                   # Source code utama untuk aset mentah dan pengembangan
├── php/                   # Skrip backend untuk menangani pemrosesan transaksi & data menu
├── css/                   # Berkas stylesheet kustom untuk estetika visual halaman
├── js/                    # Logika sisi klien untuk fungsionalitas keranjang belanja
├── img/                   # Direktori penyimpanan foto produk kopi, makanan, & background
└── index.html             # Gerbang masuk utama (Landing Page & Antarmuka Pemesanan)
```

---

## 🧠 Alur & Mekanisme Sistem Backend

Karena proyek ini didominasi oleh **PHP (74.0%)**, sistem bekerja dengan metode pemrosesan asinkronus terintegrasi:

```text
[Pelanggan Pilih Menu] ➔ [Kalkulasi di JS Cart] ➔ [Kirim Form via AJAX/POST]
                                                             │
[Halaman Konfirmasi]   🎰 [Validasi & Catat Data] 🎛️ [Diterima Skrip PHP]
```

1. **Menu Ingestion**: Sistem PHP bertugas merender atau memvalidasi ketersediaan stok produk sebelum pelanggan menekan tombol order.
2. **Order Processor**: Formulir pesanan yang dikirimkan klien akan dibongkar, disanitasi dari celah keamanan, lalu diproses di dalam folder `php/` untuk kalkulasi final nota belanja.

---

## 💻 Instalasi & Pengoperasian Lokal

Karena proyek ini menggunakan pemrosesan sisi server berbasis **PHP**, Anda membutuhkan lingkungan server lokal untuk menjalankannya:

1. **Siapkan Web Server Lokal**
   Unduh dan jalankan aplikasi server seperti **XAMPP**, **Laragon**, atau **MAMP**.
2. **Clone Repositori**
   Letakkan folder proyek ini ke dalam direktori publik server Anda (misal pada XAMPP: `C:/xampp/htdocs/`).
   ```bash
   git clone https://github.com
   ```
3. **Jalankan Proyek**
   * Aktifkan modul **Apache** pada panel kontrol XAMPP/Laragon Anda.
   * Buka browser dan akses tautan lokal: `http://localhost/kedai-ngopi-lah/`

---
Dikembangkan dengan penuh energi ☕ oleh [chochocookies](https://github.com/chochocookies).
