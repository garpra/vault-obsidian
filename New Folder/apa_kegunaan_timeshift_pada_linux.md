---
source: Chatgpt
created: 2023-04-20T14:30:00
tags:
  - resource
  - ai
  - linux
  - timeshift
  - filesystem
---

### Poin Penting
Timeshift adalah sebuah alat di Linux yang digunakan untuk membuat dan mengelola snapshot sistem. Snapshot ini berfungsi seperti cadangan (backup) dari sistem operasi, termasuk konfigurasi dan file penting, tetapi tidak mencadangkan data pengguna seperti dokumen pribadi secara default.

Timeshift memungkinkan pengguna untuk:

1. Membuat snapshot secara manual atau otomatis sesuai jadwal.
2. Mengembalikan sistem ke kondisi sebelumnya jika terjadi kesalahan atau kerusakan sistem.
3. Mendukung snapshot berbasis **RSYNC** dan **BTRFS** (untuk sistem file BTRFS dengan fitur snapshot bawaan).

Timeshift sering digunakan untuk mencegah kehilangan sistem setelah melakukan pembaruan atau perubahan besar pada sistem operasi.

### Insight Pribadi
- Dengan timeshift dimana bisa melakukan snapshot sangat membantu saya, karena saya sering menginstall ulang sistem operasi saat terjadi kesalahan karena saya sering oprek-oprek sistem linux saya.
- Karena saya menggunakan file sistem BTRFS maka timeshift bisa di terapkan pada sistem saya

### Terhubung dengan
- [[linux]]
- [[sistem_operasi]]
- [[file_sistem]]