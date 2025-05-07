---
tags:
  - topic/linux
  - topic/cachyos
---

## Sesudah Instalasi

1. Ganti default shell ke bash terlebih dahulu untuk menghapus konfigurasi bawaan fish dari CachyOS
	```bash
	chsh -s /bin/bash
	```

2. Logout dengan command
	```bash
	exit
	```

3. Login ulang denga memasukkan username dan password

4. Menghubungkan wifi dengan command
	```bash
	nmcli d wifi connect <SSID> password <PASSWORD>
	```

5. Hapus package fish beserta dependency
	```bash
	sudo pacman -Rnsc fish
	```

6. Install package yang digunakan, yang terhapus setelah hapus package fish
	```bash
	sudo pacman -S eza fastfetch fzf pkgfile fish
	```

7. Hapus folder konfigurasi bawaan fish
	```bash
	rm -rf .config/fish
	```

8. Kembalikan shellnya menjadi fish
	```bash
	chsh -s /bin/fish
	```

9. Install AUR
	```bash
	sudo pacman -S yay
	```

10. Clone dotfiles pribadi dari github
	```bash
	git clone --filter=blob:none --no-checkout https://github.com/garpra/dotfiles.git ~/.dotfiles
	
	# Pindah ke folder .dotfiles/
	cd ~/.dotfiles
	
	# Ambil folder hyprland pada dotfiles
	git sparse-checkout init --cone
	git sparse-checkout set hyprland
	git checkout main
	```

11. Install packages yang diperlukan untuk wm Hyprland
	```bash
	# Core
	sudo pacman -S hyprpaper hyprpicker brightnessctl cliphist polkit-gnome hyprland waybar ttf-0xproto-nerd
	
	# Tool
	sudo pacman -S alacritty dunst fastfetch mpv yt-dlp rofi-wayland zoxide starship
	
	# File manager
	sudo pacman -S thunar file-roller thunar-archive-plugin gvfs tumbler
	```

12. Install stow untuk management dotfile beserta setupnya
	```bash
	sudo pacman -S stow
	
	# Pindah ke folder .dotfiles/ dan buat symlink
	stow hyprland
	
	# Pastikan konfigurasi yang dimiliki sudah dihapus agar tidak terjadi konflik
	```

13. Reboot Laptop

### Terkait
- [[tujuan]]
- [[step-by-step]]
- [[04_Projects/Instalasi CachyOS/log-dev]]