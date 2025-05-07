---
tags:
  - topic/linux
  - topic/cachyos
---

## Konfigurasi

### Rekomendasi
Buka CachyOS Hello dan pergi ke bagian **App/Tweaks** dan jalankan script: Clear packages cache, Remove orphans, dan Rank Mirror

### Setup sched_ext
Buka CachyOS Kernel Manager dan pergi ke bagian **sched-ext scheduler config** dan pilih schedulernya **scx_lavd** dan profilenya **Auto**

### Setup snapper
Berguna untuk membuat rollback sistem
Buka CachyOS Hello dan pergi ke bagian **App/Tweaks** dan jalankan script Install Snapper support, setelah selesai buka Btrfs Assistant dan ke Snapper Settings matikan Snapper cleanup enabled dan apply systemd changes

### Terkait
- [[tujuan]]
- [[step-by-step]]
- [[04_Projects/Instalasi CachyOS/log-dev]]