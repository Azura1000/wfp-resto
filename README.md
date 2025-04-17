# 🍽️ WFP Resto - Laravel Food Ordering System

WFP Resto adalah aplikasi sistem pemesanan makanan berbasis web menggunakan Laravel. Sistem ini mendukung pengelolaan data makanan, kategori, pelanggan, pesanan, dan laporan statistik.

## 🚀 Fitur Utama

- Manajemen Master Data:
  - ✅ Kategori Makanan
  - ✅ Daftar Makanan
  - ✅ Data Pelanggan
  - ✅ Order / Pemesanan
- CRUD untuk semua data
- Laporan:
  - 📊 Kategori dengan jumlah makanan terbanyak
  - 📦 Makanan paling sering dipesan
  - 👥 Pelanggan dengan total pesanan tertinggi
  - 💸 Total omzet berdasarkan tanggal
- Pencarian & Filter
- Validasi Form
- Seeder dan migrasi database otomatis

## 🧰 Teknologi

- Laravel 10+
- MySQL
- Bootstrap / Tailwind (opsional untuk styling)
- Laravel Seeder, Factory, dan Migration

## ⚙️ Instalasi
1. **Clone repo:**
   ```bash
   git clone https://github.com/username/wfp_resto.git
   cd wfp_resto
   
2. **Install dependency:**
    composer install
   
3. **Copy file .env:**
    cp .env.example .env

4. **Atur konfigurasi database di file .env:**
    DB_DATABASE=wfp_resto
    DB_USERNAME=root
    DB_PASSWORD=
   
5. **Generate app key:**
    php artisan key:generate

6. **Jalankan migrasi & seeder:**
    php artisan migrate --seed

7. **Jalankan server lokal:**
    php artisan serve

8. Buka http://localhost:8000 di browser.

## 📁 Struktur Database
    categories: data kategori makanan
    foods: data makanan
    customers: data pelanggan
    orders: data pemesanan makanan
    Relasi: foods.category_id, orders.food_id, orders.customer_id

## 📃 Lisensi
Proyek ini bebas digunakan untuk keperluan pembelajaran. Silakan fork dan kembangkan lebih lanjut! ❤️
