# Identitas 
- NPM : 2210010376
- Nama : Rahmi Hidayah  
- Kelas : 5B NONREG BJM

# 📚 Aplikasi Pengelola Kontak (Java Swing & Database)

Aplikasi desktop sederhana yang dibangun menggunakan **Java Swing** untuk antarmuka grafis dan menggunakan **Database** (kemungkinan SQLite atau sejenisnya, berdasarkan adanya `Database.createDatabase()` dan kelas `Contact`) untuk menyimpan data kontak. Aplikasi ini memungkinkan pengguna untuk mengelola daftar kontak dengan operasi **CRUD** (Create, Read, Update, Delete) serta fungsionalitas pencarian, impor, dan ekspor data.

## ✨ Fitur Utama

  * **Pencatatan Kontak (CRUD):** Tambah, lihat, ubah, dan hapus data kontak (Nama, Nomor Telepon, Kategori).
  * **Tampilan Tabel:** Menampilkan daftar semua kontak dalam format tabel yang mudah dibaca.
  * **Pencarian Kontak:** Fitur pencarian untuk menemukan kontak dengan cepat.
  * **Validasi Input:** Memastikan Nomor Telepon yang dimasukkan hanya berupa digit dan memiliki panjang antara 10-15 digit.
  * **Impor/Ekspor Data:** Mendukung impor dan ekspor data kontak, kemungkinan ke format **CSV** (berdasarkan kode `Contact.eksporKeCSV()` dan `Contact.imporDariCSV()`).
  * **Antarmuka Pengguna (UI) Interaktif:** Menggunakan event listener untuk mengisi field input secara otomatis saat baris di tabel dipilih.

## 🛠️ Persyaratan Sistem

Untuk menjalankan aplikasi ini, Anda memerlukan:

  * **Java Development Kit (JDK):** Versi 8 atau lebih tinggi.
  * **Lingkungan Pengembangan Terpadu (IDE):** Seperti NetBeans, IntelliJ IDEA, atau Eclipse (kode terlihat dihasilkan oleh editor form Swing, kemungkinan NetBeans).
  * **Database:** Membutuhkan implementasi koneksi database yang ada di kelas `Contact` dan `Database` (yang tidak disertakan dalam *snippet*). Pastikan *driver* JDBC yang sesuai sudah terpasang.

## 🚀 Cara Menginstal dan Menjalankan

### 1\. Klon Repositori

Jika kode Anda berada di repositori Git:

```bash
git clone [URL_REPOSITORI_ANDA]
cd [NAMA_FOLDER_PROYEK]
```

### 2\. Konfigurasi Proyek

1.  Buka proyek di IDE pilihan Anda (misalnya NetBeans).
2.  Pastikan semua *library* yang dibutuhkan (*dependencies*), terutama untuk **Java Swing** (`javax.swing.*`) dan **SQL** (`java.sql.*`), sudah terhubung dengan benar.
3.  Pastikan kelas **`Contact`** dan **`Database`** yang dibutuhkan untuk interaksi data (seperti `tambahKontak`, `getKontak`, `createDatabase`) sudah tersedia dan terkonfigurasi untuk database lokal Anda.

### 3\. Kompilasi dan Jalankan

1.  Lakukan kompilasi proyek di IDE Anda.
2.  Jalankan kelas **`NewJFrame.java`** (kelas utama yang berisi metode `main`).

> 

## 📋 Penggunaan

1.  **Menambahkan Kontak:**
      * Masukkan **Nama**, **Nomor Telp**, dan pilih **Kategori** pada kolom input di panel kiri.
      * Klik tombol **Tambah**.
2.  **Mengubah Kontak:**
      * Pilih baris kontak dari **Tabel Daftar Kontak**. Data akan otomatis terisi di kolom input.
      * Ubah data yang diperlukan.
      * Klik tombol **Ubah**.
3.  **Menghapus Kontak:**
      * Pilih baris kontak dari **Tabel Daftar Kontak**.
      * Klik tombol **Hapus**.
4.  **Mencari Kontak:**
      * Ketik kata kunci di **Cari Kontak** di panel kanan.
      * Klik tombol **Cari**.
5.  **Keluar Aplikasi:**
      * Klik tombol **EXIT** (akan menampilkan konfirmasi sebelum menutup aplikasi).

-----

