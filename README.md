<div align="center">

# 📘 LAPORAN PRAKTIKUM PERTEMUAN KE - 1 & 2
### 🧑‍🎓 Kholil Irsyad Marwan - 4524210110
<br>


---

# 🚀 Dasar Pemrograman Berbasis Web (PHP Native)
*Laporan ini disusun untuk memenuhi Tugas Praktikum 1 dan 2 Pemrograman Berbasis Web*  


<p align="center">
  <img src="https://img.shields.io/badge/PHP-8.2+-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP 8.2">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="VS Code">
</p>

</div>

---
## Instalasi

### 1. Clone Repositori. <br>
git clone [https://github.com/KholilIrsyadMarwan/4524210110_KHOLILIRSYADMARWAN_PBW-A-Praktikum1dan2.git]. <br>

### 2. Masuk ke Folder Proyek. <br>
cd 4524210110_KHOLILIRSYADMARWAN_PBW-A-Praktikum1dan2.<br>

### 3. Jalankan Server Lokal PHP <br>
php -S localhost:8000<br>

---

## 📑 Daftar Isi

- [🎯 Tentang Aplikasi](#-tentang-aplikasi)
- [📌 Soal Tugas Praktikum](#-soal-tugas-praktikum)
- [📝 Jawaban & Pembahasan](#-jawaban--pembahasan)
- [📑 Fitur Halaman](#-fitur-halaman)
- [✨ Fitur Utama](#-fitur-utama)
- [🛠️ Tech Stack](#️-tech-stack)
- [📸 Hasil Screenshot Tampilan Website](#-hasil-screenshot-tampilan-website)


---

## 🎯 Tentang Aplikasi

Aplikasi web sederhana berbasis **PHP Native** ini dibuat untuk mengimplementasikan konsep-konsep dasar pemrograman web, seperti penanganan form input, operasi aritmatika, struktur data array asosiatif, percabangan logika, serta manipulasi string dan keamanan dasar HTML.

---

## 📌 Soal Tugas Praktikum

1. Jalankan seluruh contoh Pertemuan 1 hingga menghasilkan output tanpa error kritis.
2. Buat minimal dua modifikasi bermakna pada program (misalnya field baru, kondisi baru, styling, query, atau validasi).
3. Tuliskan penjelasan singkat untuk lima bagian kode yang menurut Anda paling penting.
4. Sertakan screenshot sebelum dan sesudah modifikasi.
5. Tuliskan satu error yang pernah muncul, penyebabnya, dan langkah perbaikannya.

---

## 📝 Jawaban & Pembahasan

### 1. Menampilkan Output Contoh 1 (`kalkulator.php`)
Menjalankan simulasi kalkulator sederhana menggunakan operasi perkalian $5 \times 5$ .
<img width="965" height="491" alt="1" src="https://github.com/user-attachments/assets/57301803-055b-4fa7-98eb-70a4ab9e3f7d" />


### Menampilkan Output Contoh 2 (`biodata.php`)
Menampilkan data profil mahasiswa yang mencakup NIM, Nama, Program Studi, Semester, dan IPK.
<img width="975" height="490" alt="2" src="https://github.com/user-attachments/assets/bd264b61-1e4d-45ee-8c6f-31db6f8dbc5a" />


### 2. Modifikasi Program
- **Modifikasi 1:** Menambahkan *field* `'status' => 'Aktif'` pada array asosiatif `$mahasiswa`.
<img width="1188" height="414" alt="3" src="https://github.com/user-attachments/assets/76afdd55-e934-40ec-9cc3-8cf619140877" />


- **Modifikasi 2:** Menambahkan fungsi kondisi `statusSemester()` untuk menentukan tingkatan mahasiswa berdasarkan semester.
<img width="1169" height="512" alt="4" src="https://github.com/user-attachments/assets/d57ba8bf-9f71-42a5-8ecd-bd721244ae5d" />


### 3. Penjelasan 5 Bagian Kode Penting
1. **Fungsi `statusKelulusan()`:** Menentukan predikat akademik berdasarkan batas nilai IPK.<br>
<img width="580" height="26" alt="5" src="https://github.com/user-attachments/assets/f53d2e3b-8920-4a6a-be6f-a9c29a9a8f23" />

2. **Array Asosiatif `$mahasiswa`:** Menyimpan data biodata mahasiswa dalam format pasangan *key-value*.<br>
<img width="275" height="128" alt="6" src="https://github.com/user-attachments/assets/c4654243-d4f9-4a30-8a61-a599bf9fddbf" />


3. **Perulangan `foreach`:** Mengiterasi seluruh pasangan *key* dan *value* dari array `$mahasiswa` untuk ditampilkan ke HTML.<br>
<img width="365" height="19" alt="7" src="https://github.com/user-attachments/assets/8d363667-4a42-499f-8b96-bb272c6ef2c9" />

4. **Percabangan `if`:** Evaluasi kondisi untuk menentukan status tingkatan semester mahasiswa.<br>
<img width="358" height="56" alt="8" src="https://github.com/user-attachments/assets/29c55678-2283-49eb-8a46-3fcc9abb65e9" />


5. **Fungsi `htmlspecialchars()`:** Mengonversi karakter khusus menjadi entitas HTML guna mencegah ancaman keamanaan Cross-Site Scripting (XSS).<br>
<img width="308" height="19" alt="9" src="https://github.com/user-attachments/assets/40a214d8-876a-4901-817e-5dfb2545b2ea" />

### 4. Tampilan Biodata Sebelum Modifikasi
Tampilan awal yang hanya memuat NIM, Nama, Prodi, Semester, IPK, dan Predikat:<br>
<img width="489" height="486" alt="Tambahan1" src="https://github.com/user-attachments/assets/99aa8c11-7e41-4918-9f68-910350ddedca" />

### Tampilan Biodata Sesudah Modifikasi
Tampilan setelah penambahan field **Status: Aktif** dan **Status Semester: Mahasiswa Tingkat Lanjut**:<br>
<img width="975" height="533" alt="Tambahan2" src="https://github.com/user-attachments/assets/5ecd4f81-c2ce-4ca1-842a-4862a7dead33" />


### 5 Error yang pernah muncul, penyebabnya, dan langkah perbaikannya
- **Penyebab:** Terjadi *typo* pada nama fungsi saat dipanggil (`statuselulusan`), yang tidak sesuai dengan deklarasi fungsi `statusKelulusan()`.<br>
<img width="746" height="60" alt="12" src="https://github.com/user-attachments/assets/e8f527d6-fce2-4683-952a-071914fe69d6" />


- **Perbaikan:** Memperbaiki penulisan nama fungsi pada saat pemanggilan agar sesuai dengan deklarasi awal, yaitu `statusKelulusan()`.<br>
<img width="309" height="79" alt="13" src="https://github.com/user-attachments/assets/1d3ded67-29d4-43db-9357-a49f0917827a" />


---

## 📑 Fitur Halaman

Aplikasi ini terdiri dari 2 file utama:

1. **Kalkulator Sederhana (`kalkulator.php`)**
   - Menyediakan form input angka dan pilihan operator aritmatika ($+, -, *, /$).<br>

2. **Biodata Mahasiswa (`biodata.php`)**
   - Menampilkan ringkasan informasi biodata, predikat IPK, dan kategori semester secara dinamis.<br>
   
3. **Biodata Mahasiswa (`biodata.php`)** <br>
   - Menambahkan field **Status: Aktif** dan **Status Semester: Mahasiswa Tingkat Lanjut**.<br>
---

## ✨ Fitur Utama

- ✅ **Perhitungan Aritmatika (`kalkulator.php`)** - Mendukung operasi dasar kalkulator.
- ✅ **Dynamic Biodata Rendering (`biodata.php`)** - Menampilkan list biodata dari array asosiatif.
- ✅ **Kategori Semester Otomatis** - Menentukan status mahasiswa (Baru, Menengah, Tingkat Lanjut) berdasarkan input semester.
- ✅ **Evaluasi Predikat IPK** - Menghasilkan predikat kelulusan berdasarkan range IPK.
- ✅ **Keamanan Output HTML** - Menggunakan `htmlspecialchars()` pada output string.

---

## 🛠️ Tech Stack

### Backend & Core
- **PHP 8.2+** - Native Scripting Language.

### Frontend
- **HTML5** - Markup Structure.
- **CSS3** - Basic Styling.

---

## 📸 Hasil Screenshot Tampilan Website

### 1. Tampilan Kalkulator  (`kalkulator.php`)
Output hasil perhitungan perkalian $5 \times 5$:
<img width="1336" height="262" alt="kalkulator" src="https://github.com/user-attachments/assets/0c06e45a-2f6b-4a63-8387-6880258250ee" />

---

### 2. Tampilan Biodata (`biodata.php`)
Tampilan awal yang hanya memuat NIM, Nama, Prodi, Semester, IPK, dan Predikat:
<img width="1600" height="275" alt="biodata" src="https://github.com/user-attachments/assets/b941a78b-5e87-4cf4-97cc-1e9e6ca2a5c8" />

---

### 3. Tampilan Biodata (`biodataupdate.php`)
Tampilan setelah penambahan field **Status: Aktif** dan **Status Semester: Mahasiswa Tingkat Lanjut**:
<img width="1600" height="373" alt="biodataupdate" src="https://github.com/user-attachments/assets/4223678a-a44b-460a-9e63-3d22388f3f7b" />


---


