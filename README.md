<div align="center">

# 📘 LAPORAN PRAKTIKUM PERTEMUAN KE - 4
### 🧑‍🎓 Kholil Irsyad Marwan - 4524210110
<br>

# 🚀 Website LaraPress (Autentikasi & Proteksi Route)
*Laporan ini disusun untuk memenuhi Tugas Praktikum 4 Pemrograman Berbasis Web*

<p align="center">
  <img src="https://img.shields.io/badge/Laravel-11.x-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel 11">
  <img src="https://img.shields.io/badge/PHP-8.2+-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP 8.2">
  <img src="https://img.shields.io/badge/Tailwind_CSS-3.x-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS">
  <img src="https://img.shields.io/badge/Laravel_Breeze-Auth-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel Breeze">
</p>

</div>

---
## 📑 Daftar Isi

- [🎯 Tentang Aplikasi](#-tentang-aplikasi)
- [📌 Soal Tugas Praktikum](#-soal-tugas-praktikum)
- [📝 Jawaban & Pembahasan](#-jawaban--pembahasan)
- [📑 Fitur Halaman](#-fitur-halaman)
- [✨ Fitur Utama](#-fitur-utama)
- [🛠️ Tech Stack](#️-tech-stack)
- [📸 Hasil Screenshot Tampilan Website LaraPress](#-hasil-screenshot-tampilan-website-larapress)
- [⚙️ Cara Menjalankan Proyek](#️-cara-menjalankan-proyek)

---
## 🎯 Tentang Aplikasi

**LaraPress** pada Praktikum 4 ini dikembangkan berbasis **Laravel 11** dan **Laravel Breeze** untuk mengimplementasikan sistem autentikasi pengguna (*Register, Login, Dashboard, Profile*) serta mekanisme keamanan proteksi rute CRUD menggunakan middleware `auth`.

---

## 📌 Soal Tugas Praktikum

1. **Logout** dari aplikasi Anda.<br> Sekarang, coba akses URL untuk membuat postingan baru: `http://127.0.0.1:8000/posts/create`.<br> **Apa yang terjadi?** Laravel akan secara otomatis mengarahkan Anda ke halaman login!

---

## 📝 Jawaban & Pembahasan

### 1. Mengakses URL Pembuatan Postingan Baru (`http://127.0.0.1:8000/posts/create`)
Ketika mencoba mengakses URL pembuatan postingan baru (`http://127.0.0.1:8000/posts/create`) dalam kondisi belum terotentikasi (logout), middleware Laravel secara otomatis mengalihkan pengguna ke halaman login (`http://127.0.0.1:8000/login`).

<img width="1600" height="757" alt="Login Baru" src="https://github.com/user-attachments/assets/ce27bcaa-0ce3-4669-91c0-4c9429f6474e" />

---

## 📑 Fitur Halaman

Aplikasi web ini memiliki beberapa halaman utama dan rute terproteksi:

1. **Halaman Register (`/register`)**
   - Menampilkan formulir pendaftaran akun pengguna baru ke dalam sistem.
2. **Halaman Login (`/login`)**
   - Menampilkan formulir masuk bagi pengguna terdaftar menggunakan email dan password.
3. **Halaman Dashboard (`/dashboard`)**
   - Halaman utama pengguna terautentikasi setelah berhasil melakukan login.
4. **Halaman Profile (`/profile`)**
   - Menampilkan pengaturan profil pengguna, pembaruan kata sandi, dan opsi penghapusan akun.
5. **Rute Tambah Postingan (`/posts/create`)**
   - Rute pembuatan postingan baru yang dilindungi middleware `auth` dan otomatis me-redirect ke `/login` jika diakses tanpa sesi aktif.

---

## ✨ Fitur Utama

- ✅ **Sistem Autentikasi Pengguna (Laravel Breeze)** - Fitur pendaftaran akun, login, dan pengakhiran sesi (*logout*) secara aman.
- ✅ **Proteksi Route Middleware `auth`** - Mengamankan rute sensitif seperti `/posts/create` dari akses anonim/pengguna tanpa izin.
- ✅ **Manajemen Profil Pengguna** - Pengelolaan data akun pribadi, keamanan kata sandi, dan fitur hapus akun.
- ✅ **Dashboard Terproteksi** - Antarmuka khusus pengguna terdaftar setelah terautentikasi.

---

## 🛠️ Tech Stack

### Backend & Framework
- **Laravel 11.x** - PHP Framework
- **PHP ^8.2** - Programming Language
- **Laravel Breeze** - Authentication Package
- **Blade Engine** - Templating System

### Frontend
- **Tailwind CSS** - CSS Framework
- **Responsive Layout** - Modern UI Design

---

## 📸 Hasil Screenshot Tampilan Website LaraPress

### 1. Halaman Register (`/register`)
<img width="1600" height="812" alt="Register" src="https://github.com/user-attachments/assets/2a30ad11-6ab2-4df2-861e-54a9b5a61377" />

---

### 2. Halaman Login (`/login`)
<img width="1600" height="757" alt="Login Baru" src="https://github.com/user-attachments/assets/a328efef-17ce-48f9-b6f6-13480169908a" />

---

### 3. Halaman Dashboard (`/dashboard`)
<img width="1600" height="808" alt="Dashboard" src="https://github.com/user-attachments/assets/739deef4-a4b4-4b1a-984c-ede828d772db" />

---

### 4. Halaman Profile (`/profile`)
<img width="1600" height="577" alt="Profile 1" src="https://github.com/user-attachments/assets/8fa6968c-7ec1-4ceb-80a2-26d700e6810d" /> <br>
<img width="1600" height="793" alt="Profile 2" src="https://github.com/user-attachments/assets/4e90a463-fdc5-4cfe-8048-e48d56bfff15" />

---
## ⚙️ Cara Menjalankan Proyek

1. Clone Repositori<br>
git clone [https://github.com/KholilIrsyadMarwan/4524210110_KHOLILIRSYADMARWAN_PBW-A-Praktikum4.git].
2. Masuk ke Folder Proyek<br>
cd 4524210110_KHOLILIRSYADMARWAN_PBW-A-Praktikum4<br>
3. Install Dependensi & Set Up Environment <br>
composer install<br>
npm install<br>
cp .env.example .env<br>
php artisan key:generate<br>
4. Jalankan Aplikasi<br>
npm run dev<br>
php artisan serve<br>
