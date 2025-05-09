---
source: https://wiki.archlinux.org/title/Polkit
author: archlinux
tags:
  - linux
  - os
  - polkit
---

## Judul: Contoh Penggunaan Authorization rules pada Polkit

### Ringkasan
Untuk mengizinkan anggota grup `wheel` menjalankan GParted dan Libvirt tanpa otentikasi, Buat file `/etc/polkit-1/rules.d/49-wheel-allow-gparted-libvirt.rules` dengan isi:
```javascript
	polkit.addRule(function(action, subject) {
	    if ((action.id == "org.gnome.gparted" ||
	        action.id == "org.libvirt.unix.manage") &&
	        subject.isInGroup("wheel")) {
	        return polkit.Result.YES;
	    }
	});
```

### Terkait dengan
- [[linux]]
- [[sistem_operasi]]
- [[L-Polkit dan perbedaannya dengan sudo]]
- [[L-Konfigurasi pada Polkit]]
- [[L-Peran Authentication agent dalam Polkit]]

