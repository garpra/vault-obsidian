---
tags:
  - topic/linux
  - topic/cachyos
---

## Step by Step Instalasi CachyOS

1. Buat bootable USB untuk cachyos iso
	```bash
	sudo dd if=cachyos.iso of=/dev/sda bs=4M status=progress
	```
2. Menghubungkan wifi dan "Manually Block" pada setting Power & Battery supaya layar tidak mati selama proses instalasi
3. Tekan Launch Installer dan tunggu sesaat
4. Pilih Bootloader: GRUB
5. Pilih bahasa: America English
6. Pilih Region & Zone: Asia Jakarta
7. Pilih Keyboard: English(US) Default
8. Bagian Lartition pilih **"Erase disk"** dengan filesystem **"Btrfs"**
9. Pilih DE atau WM, saya memilih Hyprland
10. Pilih package yang diperlukan --> [[package-pilihan]]
11. Isikan nama anda, nama komputer, dan password
12. Tunggu instalasi selesai, proses akan cukup lama tergantung koneksi internet
13. Shutdown CachyOS dan cabut flashdisk
14. Nyalakan Laptop dan login ke Akun yang sudah dibuat

### Terkait
- [[tujuan]]
- [[post-instalasi]]
- [[tweaks]]
- [[04_Projects/Instalasi CachyOS/log-dev]]
