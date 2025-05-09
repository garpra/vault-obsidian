---
source: Chatgpt
created: 23-04-2025 18-05
tags:
  - resource
  - ai
  - cli
---

### Poin Penting
Untuk menyambung ke jaringan Wi-Fi menggunakan `nmcli`, ikuti langkah-langkah berikut:

#### 1. Daftar Jaringan yang Tersedia

Jalankan perintah berikut untuk memindai dan menampilkan jaringan Wi-Fi terdekat:
```bash
nmcli dev wifi list
```

#### 2. Menyambungkan ke Jaringan Wi-Fi

Gunakan SSID (nama jaringan Wi-Fi) dan kata sandi (jika diperlukan) untuk menyambung:
```bash
nmcli dev wifi connect “<SSID>” password “<password>”
```

Sebagai contoh:
```bash
nmcli dev wifi connect “MyWiFi” kata sandi “mypassword123”
```

Jika jaringan terbuka (tanpa kata sandi), jalankan saja:
```bash
nmcli dev wifi sambungkan “MyWiFi”
```

#### 3. Memverifikasi Sambungan

Periksa apakah Anda tersambung ke jaringan:
``` bash
nmcli connection show --active
```

#### Tips Tambahan:

- **Menyambung kembali ke jaringan yang tersimpan:**
    Jika Anda pernah tersambung ke jaringan sebelumnya, Anda dapat menyambung kembali:
```bash
nmcli connection up “<SSID>”
```

- **Melupakan jaringan:**
    Untuk menghapus sambungan Wi-Fi yang tersimpan:
```bash
nmcli connection delete “<SSID>”
```

### Terhubung dengan
- [[linux]]
- [[cli]]