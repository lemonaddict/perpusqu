# 📚 PerpusQu - Aplikasi Manajemen Perpustakaan

PerpusQu adalah aplikasi desktop sederhana yang dibuat dengan Java Swing untuk mengelola peminjaman dan pengembalian buku di perpustakaan. Proyek ini dibuat sebagai latihan untuk memahami koneksi database Java (JDBC) dan GUI Swing.

## ✨ Fitur-fitur
* Login User (menggunakan Nama dan NIM)
* Melihat daftar buku yang tersedia
* Meminjam buku (Stok buku akan berkurang)
* Melihat daftar buku yang sedang dipinjam (spesifik per user)
* Mengembalikan buku (Stok buku akan bertambah dan status update)
* Perhitungan denda otomatis jika pengembalian telat.

## 🛠️ Teknologi yang Digunakan
* **Java (JDK 20)**
* **Java Swing** (untuk Grapichal User Interface / GUI)
* **MySQL** (via XAMPP)
* **JDBC** (untuk koneksi Java ke MySQL)

## 🚀 Cara Menjalankan Proyek

Untuk menjalankan proyek ini di komputermu, ikuti langkah-langkah berikut:

**1. Prasyarat**
* Pastikan kamu sudah menginstal [Java JDK](https://www.oracle.com/java/technologies/downloads/) (proyek ini dibuat menggunakan JDK 20).
* Pastikan kamu sudah menginstal [XAMPP](https://www.apachefriends.org/index.html) dan menjalankan service **Apache** dan **MySQL**.
* IDE [Apache NetBeans](https://netbeans.apache.org/download/index.html).

**2. Setup Database**
1.  Buka **phpMyAdmin** (`http://localhost/phpmyadmin`).
2.  Buat database baru dengan nama `perpusqu`.
3.  Pilih database `perpusqu`, lalu klik tab **"Import"**.
4.  Klik "Choose File" dan pilih file `database/perpusqu (1).sql` dari proyek ini.
5.  Klik "Go" atau "Import" di bagian bawah. Database-mu sekarang sudah siap.

**3. Setup Proyek**
1.  Clone repositori ini:
    ```bash
    git clone [https://github.com/lemonaddict/PerpusQu.git](https://github.com/lemonaddict/PerpusQu.git)
    ```
2.  Buka proyek `PerpusQu` di NetBeans.
3.  (Jika kamu pakai *config.properties*) Salin file `config.example.properties` dan ganti namanya menjadi `config.properties`.
4.  (Jika kamu pakai *config.properties*) Buka `config.properties` dan masukkan password database MySQL-mu (jika ada).
5.  Tambahkan `mysql-connector-j-8.2.0.jar` (atau versi terbarumu) ke **Libraries** proyek di NetBeans. (Klik kanan Libraries > Add JAR/Folder...).

**4. Jalankan!**
* Klik kanan proyek `PerpusQu` di NetBeans dan pilih **"Clean and Build"**.
* Setelah selesai, klik kanan lagi dan pilih **"Run"**.
* Aplikasi akan terbuka di halaman Login.

**Contoh Akun untuk Login (dari database):**
* **Nama:** Admin
* **NIM:** admin
