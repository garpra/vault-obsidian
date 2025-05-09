---
source: Chatgpt
created: 23-04-2025 17-47
tags:
  - resource
  - ai
  - cli
---

### Poin Penting
Perintah `iwctl` merupakan bagian dari paket iwd (iNet Wireless Daemon), yang digunakan untuk mengelola jaringan nirkabel pada sistem Linux, termasuk archlinux. Di bawah ini adalah panduan singkat untuk menggunakan iwctl untuk menyambung ke jaringan Wi-Fi:

#### 1. Buka iwctl
Jalankan perintah berikut untuk memulai shell interaktif `iwctl`:
```bash
iwctl
```

#### 2. Buat daftar perangkat Wi-Fi yang tersedia
Di dalam shell `iwctl`, gunakan perintah ini untuk membuat daftar perangkat nirkabel Anda:
```bash
device list
```

Catat nama perangkat Wi-Fi Anda (misalnya, `wlan0`).

#### 3. Memindai Jaringan yang Tersedia
Ganti `<device>` dengan nama perangkat Anda (misalnya, `wlan0`):
```bash
station <device> scan
```

Setelah pemindaian, Anda dapat membuat daftar jaringan:
```bash
station <device> get-networks
```

### 4. Menyambungkan ke Jaringan
Gunakan perintah berikut untuk menyambung ke jaringan. Ganti `<SSID>` dengan nama jaringan:
```bash
stasiun <device> sambungkan <SSID>''
```

Jika jaringan memerlukan kata sandi, Anda akan diminta untuk memasukkannya.

### 5. Memeriksa Status Sambungan
Verifikasi status koneksi:
```bash
station <device> show
```

### 6. Keluar dari iwctl
Untuk keluar dari shell `iwctl`, ketik:
```bash
exit
```

### Terhubung dengan
- [[linux]]
- [[cli]]