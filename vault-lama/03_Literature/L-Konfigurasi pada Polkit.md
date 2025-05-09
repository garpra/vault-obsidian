---
source: https://wiki.archlinux.org/title/Polkit
author: archlinux
tags:
  - linux
  - os
  - polkit
---

## Judul: Konfigurasi pada Polkit

### Ringkasan
Konfigurasi polkit dapat dibagi menjadi dua jenis:

1. Actions (Tindakan)
	- Akan tersimpan dalam file XML dengan format `.policy`. 
	- Terletak di folder `/usr/share/polkit-1/actions`.
	- Menyimpan tindakan dengan ID Unik
	- Pengaturan izin default disimpan disini
	- Tidak disarankan untuk langsung mengatur konfigurasi dari file `.policy`
2. Authorization rules
	- Ditulis dalam bahasa pemrograman Javascript dengan format `.rules`
	- Ditempatkan dalam folder `/etc/polkit-1/rules.d` untuk konfigurasi lokal
	- Menggunakan fungsi `polkit.addRule()` untuk menentukan apakah diizinkan atau ditolak untuk melakukan tindakan tertentu.

### Terkait dengan
- [[linux]]
- [[sistem_operasi]]
- [[L-Polkit dan perbedaannya dengan sudo]]
- [[L-Contoh Penggunaan Authorization rules pada Polkit]]
- [[L-Peran Authentication agent dalam Polkit]]

