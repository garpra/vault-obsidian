# 📘 Daftar Keybind Tmux Paling Sering Digunakan

> Default prefix: `Ctrl + b`  
> Tekan `Ctrl + b`, lalu tekan tombol berikutnya.

---

## 🔧 Dasar

| Keybind         | Fungsi                                  |
|-----------------|------------------------------------------|
| `c`             | Membuat window baru                      |
| `n`             | Pindah ke window berikutnya              |
| `p`             | Pindah ke window sebelumnya              |
| `l`             | Pindah ke window terakhir                |
| `&`             | Menutup window saat ini                  |
| `,`             | Ganti nama window                        |
| `w`             | Pilih window dari daftar                 |
| `f`             | Cari window berdasarkan nama             |
| `d`             | Detach dari sesi tmux                    |
| `s`             | Lihat daftar sesi                        |
| `$`             | Ganti nama sesi                          |
| `?`             | Tampilkan semua keybind                  |
| `:`             | Masuk ke mode command prompt             |

---

## 🧱 Panel / Split

| Keybind         | Fungsi                                  |
|-----------------|------------------------------------------|
| `%`             | Split vertikal (kanan-kiri)              |
| `"`             | Split horizontal (atas-bawah)            |
| `x`             | Tutup panel                              |
| `o`             | Pindah antar panel                       |
| `{` / `}`       | Tukar posisi panel ke kiri / kanan       |
| `Space`         | Ganti layout panel                       |
| `!`             | Pop-out panel menjadi window             |
| `Ctrl + o`      | Rotasi posisi panel                      |
| `;`             | Kembali ke panel sebelumnya              |
| `q`             | Tampilkan nomor panel sementara          |
| `z`             | Zoom panel (maximize/minimize)           |

---

## ⌨️ Navigasi Panel (Arrow)

| Keybind         | Fungsi                                  |
|-----------------|------------------------------------------|
| `← ↑ ↓ →`       | Navigasi antar panel (setelah prefix)   |

---

## 📜 Copy Mode

| Keybind         | Fungsi                                  |
|-----------------|------------------------------------------|
| `[`             | Masuk ke copy mode                       |
| `↑ / ↓`         | Navigasi baris                           |
| `PgUp / PgDn`   | Navigasi halaman                         |
| `Space`         | Mulai pemilihan teks                     |
| `Enter`         | Salin teks ke buffer tmux                |
| `q`             | Keluar dari copy mode                    |

---

## 📋 Buffer & Paste

| Keybind         | Fungsi                                  |
|-----------------|------------------------------------------|
| `]`             | Paste isi buffer                         |
| `=`             | Pilih buffer yang ingin dipaste          |

---

## 🧰 Manajemen Session via Terminal

```sh
tmux new -s nama_sesi       # Membuat sesi baru
tmux ls                     # Melihat daftar sesi
tmux attach -t nama_sesi    # Masuk ke sesi
tmux kill-session -t nama   # Menghapus sesi
```

