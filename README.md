<div align="center">

# 📘 LAPORAN PRAKTIKUM PERTEMUAN KE - 1 & 2
### 🧑‍🎓 Kholil Irsyad Marwan - 4524210110
<br>

# 🚀 Dasar Pemrograman Berbasis Web (PHP Native)
*Laporan ini disusun untuk memenuhi Tugas Praktikum 1 dan 2 Pemrograman Berbasis Web*  
*Dosen Pengampu: Bambang Riono Arsad, S.Kom., MMSI*

<p align="center">
  <img src="https://img.shields.io/badge/PHP-8.2+-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP 8.2">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="VS Code">
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
- [📸 Hasil Screenshot Tampilan Website](#-hasil-screenshot-tampilan-website)
- [⚠️ Penanganan Error](#️-penanganan-error)
- [⚙️ Cara Menjalankan Proyek](#️-cara-menjalankan-proyek)

---

## 🎯 Tentang Aplikasi

Aplikasi web sederhana berbasis **PHP Native** ini dibuat untuk mengimplementasikan konsep-konsep dasar pemrograman web, seperti penanganan form input, operasi aritmatika, struktur data array asosiatif, percabangan logika, serta manipulasi string dan keamanan dasar HTML.

---

## 📌 Soal Tugas Praktikum

1. Jalankan seluruh contoh Pertemuan 1 hingga menghasilkan output tanpa error kritis[cite: 1].
2. Buat minimal dua modifikasi bermakna pada program (misalnya field baru, kondisi baru, styling, query, atau validasi)[cite: 1].
3. Tuliskan penjelasan singkat untuk lima bagian kode yang menurut Anda paling penting[cite: 1].
4. Sertakan screenshot sebelum dan sesudah modifikasi[cite: 1].
5. Tuliskan satu error yang pernah muncul, penyebabnya, dan langkah perbaikannya[cite: 1].

---

## 📝 Jawaban & Pembahasan

### 1. Menampilkan Output Contoh 1 (`kalkulator.php`)
Menjalankan simulasi kalkulator sederhana menggunakan operasi perkalian ($5 \times 5 = 25$)[cite: 1].

### 2. Menampilkan Output Contoh 2 (`biodata.php`)
Menampilkan data profil mahasiswa yang mencakup NIM, Nama, Program Studi, Semester, dan IPK[cite: 1].

### 3. Modifikasi Program
- **Modifikasi 1:** Menambahkan *field* `'status' => 'Aktif'` pada array asosiatif `$mahasiswa`[cite: 1].
- **Modifikasi 2:** Menambahkan fungsi kondisi `statusSemester()` untuk menentukan tingkatan mahasiswa berdasarkan semester[cite: 1].

### 4. Penjelasan 5 Bagian Kode Penting
1. **Fungsi `statusKelulusan()`:** Menentukan predikat akademik berdasarkan batas nilai IPK[cite: 1].
2. **Array Asosiatif `$mahasiswa`:** Menyimpan data biodata mahasiswa dalam format pasangan *key-value*[cite: 1].
3. **Perulangan `foreach`:** Mengiterasi seluruh pasangan *key* dan *value* dari array `$mahasiswa` untuk ditampilkan ke HTML[cite: 1].
4. **Percabangan `if`:** Evaluasi kondisi untuk menentukan status tingkatan semester mahasiswa[cite: 1].
5. **Fungsi `htmlspecialchars()`:** Mengonversi karakter khusus menjadi entitas HTML guna mencegah ancaman keamanaan Cross-Site Scripting (XSS)[cite: 1].

---

## 📑 Fitur Halaman

Aplikasi ini terdiri dari 2 file utama:

1. **Kalkulator Sederhana (`kalkulator.php`)**[cite: 1]
   - Menyediakan form input angka dan pilihan operator aritmatika ($+, -, *, /$)[cite: 1].
2. **Biodata Mahasiswa (`biodata.php`)**[cite: 1]
   - Menampilkan ringkasan informasi biodata, predikat IPK, dan kategori semester secara dinamis[cite: 1].

---

## ✨ Fitur Utama

- ✅ **Perhitungan Aritmatika (`kalkulator.php`)** - Mendukung operasi dasar kalkulator[cite: 1].
- ✅ **Dynamic Biodata Rendering (`biodata.php`)** - Menampilkan list biodata dari array asosiatif[cite: 1].
- ✅ **Kategori Semester Otomatis** - Menentukan status mahasiswa (Baru, Menengah, Tingkat Lanjut) berdasarkan input semester[cite: 1].
- ✅ **Evaluasi Predikat IPK** - Menghasilkan predikat kelulusan berdasarkan range IPK[cite: 1].
- ✅ **Keamanan Output HTML** - Menggunakan `htmlspecialchars()` pada output string[cite: 1].

---

## 🛠️ Tech Stack

### Backend & Core
- **PHP 8.2+** - Native Scripting Language[cite: 1]

### Frontend
- **HTML5** - Markup Structure[cite: 1]
- **CSS3** - Basic Styling[cite: 1]

---

## 📸 Hasil Screenshot Tampilan Website

### 1. Tampilan Kalkulator Sederhana (`kalkulator.php`)
Output hasil perhitungan perkalian $5 \times 5$:
<img width="145" height="25" alt="4" src="https://github.com/user-attachments/assets/d86469e0-9adb-4ec7-9b41-ec606a56138e" />

---

### 2. Tampilan Biodata Sebelum Modifikasi
Tampilan awal yang hanya memuat NIM, Nama, Prodi, Semester, IPK, dan Predikat[cite: 1]:
![Biodata Sebelum Modifikasi](https://via.placeholder.com/800x400?text=Screenshot+Biodata+Sebelum+Modifikasi)[cite: 1]

---

### 3. Tampilan Biodata Sesudah Modifikasi
Tampilan setelah penambahan field **Status: Aktif** dan **Status Semester: Mahasiswa Tingkat Lanjut**[cite: 1]:
![Biodata Sesudah Modifikasi](https://via.placeholder.com/800x400?text=Screenshot+Biodata+Sesudah+Modifikasi)[cite: 1]

---

## ⚠️ Penanganan Error

- **Error:** `Call to unknown function: 'statuselulusan'`[cite: 1]
- **Penyebab:** Terjadi *typo* pada nama fungsi saat dipanggil (`statuselulusan`), yang tidak sesuai dengan deklarasi fungsi `statusKelulusan()`[cite: 1].
- **Perbaikan:** Memperbaiki penulisan nama fungsi pada saat pemanggilan agar sesuai dengan deklarasi awal, yaitu `statusKelulusan()`[cite: 1].

---

## ⚙️ Cara Menjalankan Proyek

1. **Clone / Download Repositori**
   ```bash
   git clone [https://github.com/KholilIrsyadMarwan/4524210110_KHOLILIRSYADMARWAN_PBW-A-Praktikum1dan2.git](https://github.com/KholilIrsyadMarwan/4524210110_KHOLILIRSYADMARWAN_PBW-A-Praktikum1dan2.git)
