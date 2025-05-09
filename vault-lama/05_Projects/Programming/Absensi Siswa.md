---
status: Complete
tags:
  - web
---

## Judul : Absensi Siswa
### Tujuan
Aplikasi web ini dibuat dengan tujuan sebagai pencatat absensi siswa menggunakan framework Express.js. Cocok digunakan oleh guru dan staf sekolah dalam mencatat dan mengelola kehadiran

### Fitur
- Halaman Home
	- Navigasi Bar
	- Judul Halaman
	- Tanggal saat ini
	- Table Siswa dengan berisi No, Nama, NIM, dan Absensi untuk mencatat kehadiran siswa
	- Tombol **"Save"** untuk menyimpan data siswa ke sistem
- Halaman Daftar Siswa
	- Navigasi Bar
	- Judul Halaman
	- Tombol **"Add Student"** untuk menambahkan siswa baru ke sistem
	- Tabel Siswa yang berisi No, Nama, NIM, dan Aksi untuk hapus/edit siswa
- Halaman Rekap Absensi
	- Navigasi Bar
	- Judul Halaman
	- Dropdown Bulan Rekap
	- Table Rekap Siswa berisi No, Nama, NIM, Jumlah masuk, sakit, alpha

### Alat dan Teknologi 
- HMTL
- Bootstrap
- NodeJS
- ExpressJS
- Docker

### Alur Aplikasi
- **Halaman Home**
	- Saat pengguna pertama membuka website, mereka akan diarahkan ke halaman utama.
	- Di halaman ini, pengguna dapat melihat tanggal hari ini, tabel yang berisi daftar siswa, dan absensi siswa.
	- Pengguna bisa menyimpan hasil absensi dengan menekan tombol **"Simpan"**
- **Halaman Daftar**
	- Di halaman ini, pengguna bisa melihat daftar siswa yang tersedia
	- Pengguna bisa menambahkan siswa baru ke daftar dengan menekan tombol **"Tambah Data"** dan akan dibawa ke halaman tambah siswa
	- Pengguna juga bisa mengedit dan menghapus data yang ada dengan menekan tombol di kolom Aksi, untuk tombol **"Update"** pengguna akan dibawa ke halaman edit siswa
- **Halaman Tambah Siswa**
	- Di halaman ini terdapat input nama dan nim, pengguna bisa mengisikan data sesuai yang diinginkan
	- Jika mau menyimpan data siswa pengguna bisa menekan tombol **"Simpan"** dan data akan disimpan ke daftar
	- Jika pengguna menekan tombol **"Kembali"** maka pengguna akan kembali ke halaman daftar
- **Halaman Rekap**
	- 

### Desain
-

### Timeline
- Design: 28-04-2025
- Refactoring: 28-04-2025

### Referensi
- [[absensi_siswa]]

##### Link to List
[[Programming Project]]
