---
source: Chatgpt
created: 23-04-2025 17-39
tags:
  - resource
  - ai
  - linux
---

### Poin Penting
Untuk memeriksa jika ada error di Arch Linux, berikut beberapa langkah yang bisa Anda lakukan:

#### 1. Periksa Log Sistem

Gunakan perintah **`journalctl`** untuk melihat log sistem. Ini adalah langkah pertama untuk mendiagnosis error.

- Lihat log terbaru:
```bash
journalctl -p err -b
```

Ini akan menampilkan log dengan prioritas _error_ (level `err`) untuk boot saat ini.

- Jika Anda ingin log dari semua prioritas:
```bash
journalctl -b
```

#### 2. Cek Status Layanan

Gunakan **`systemctl`** untuk memeriksa status layanan:

- Cek semua layanan yang gagal:
```bash
systemctl --failed
```

- Periksa status spesifik suatu layanan:
```bash
systemctl status <nama-layanan>
```

### 3. **Pantau Paket yang Bermasalah**

- Setelah update sistem, periksa jika ada error:
```bash
sudo pacman -Syu
```

Jika ada masalah dependensi atau konflik, pacman akan memberi tahu Anda.

- Gunakan **`pactree`** untuk melihat dependensi paket tertentu:
```bash
pactree <nama-paket>
```

### 4. **Cek File yang Hilang atau Konflik**

- Gunakan **`pacman`** untuk memverifikasi integritas semua paket:
```bash
pacman -Qk
```

Paket yang tidak lengkap akan ditandai.

### 5. **Pantau Ruang Disk**

Jika ada error terkait _disk_, pastikan tidak kehabisan ruang:
```bash
df -h
```

### 6. **Gunakan Alat Diagnostik**

- Gunakan **`dmesg`** untuk memeriksa error kernel:
```bash
dmesg | grep -i error
```

### 7. **Cek Snapper (Jika Menggunakan Btrfs)**

Karena Anda menggunakan Snapper dengan Btrfs:

- Cek snapshot:
```bash
sudo snapper list
```

- Periksa error terkait filesystem:
```bash
sudo btrfs scrub status /
```

### Terhubung dengan
- [[linux]]
