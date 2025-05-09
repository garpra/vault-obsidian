---
status: Complete
tags:
  - web
---

## Judul : Anime List
### Tujuan
Aplikasi web dibuat dengan tujuan sebagai katalog anime dan manga dari berbagai kategori yang di ambil dari Jikan API, dimana pengguna bisa mencari anime atau manga yang disukai dan menyimpannya kedalam bookmark, Aplikasi ini juga menyediakan section untuk anime yang baru rilis musim ini dan rekomendasi anime/manga yang banyak disukai pengguna.

### Fitur
- Halaman Home
	- Section Anime Season Now
	- Section Anime Recomendation
	- Section Manga Recomendation
- Halaman Anime
	- Search bar
	- List anime berdasarkan pencarian
- Halaman Manga
	- Search bar
	- List manga berdasarkan pencarian
- Halaman Expand List
	- Menampilkan lebih banyak anime/manga dari masing-masing kategori
- Halaman Bookmark
	- Daftar anime dan manga yang disimpan pengguna
	- Tombol hapus untuk mengelola bookmark

### Alat dan Teknologi 
- HTML
- CSS
- JavaScript
- JikanAPI

### Alur Aplikasi
- **Halaman Home**
    - Saat pertama kali mengakses website, pengguna akan diarahkan ke halaman home yang terdiri dari tiga section yaitu Anime Season Now, Anime Recomendation, Manga Recomendation.
    - Pengguna dapat melihat lebih banyak item dari masing-masing section dengan menekan tombol `Load More`.
	
- **Halaman Detail Anime/Manga**
    - Pengguna dapat mengklik salah satu card anime/manga dari halaman untuk masuk ke detail anime/manga.
    - Halaman ini menampilkan informasi lengkap seperti sinopsis, genre, status, episode/volume, rating, dan lainnya.
    - Di dalam halaman ini, pengguna bisa menyimpan anime/manga tersebut ke dalam daftar Bookmark.
    
- **Fitur Pencarian**
    - Terdapat halaman khusus untuk pencarian anime/manga.
    - Pengguna dapat menginputkan judul anime/manga yang ingin dicari menggunakan search bar.
    - Hasil pencarian ditampilkan dalam bentuk card.
    
- **Halaman Bookmark**
    - Semua anime/manga yang telah disimpan akan muncul di halaman Bookmark.
    - Pengguna dapat melihat koleksi pribadi mereka kapan saja dari halaman ini.

### Desain
-

### Timeline
- Redesign: 12-03-2025
- Refactoring: 12-03-2025

### Referensi
- [[anime_list]]
- [[application_programming_interface]]

##### Link to List
[[Programming Project]]
