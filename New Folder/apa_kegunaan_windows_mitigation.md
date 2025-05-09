---
source: Chatgpt
created: 23-04-2025 17-25
tags:
  - resource
  - ai
  - security
  - os
  - windows
---

### Poin Penting
Windows mitigations adalah teknik keamanan yang digunakan oleh sistem operasi Windows untuk mencegah serangan atau eksploitasi pada kerentanannya. Mitigations ini bertujuan untuk memperkuat keamanan sistem dengan mengurangi risiko yang ditimbulkan oleh perangkat lunak berbahaya (malware) atau teknik eksploitasi tertentu. Berikut beberapa kegunaan Windows mitigations:

1. **Mencegah Eksekusi Arbitrary Code**: Beberapa mitigasi seperti Data Execution Prevention (DEP) mencegah eksekusi kode di area memori yang seharusnya hanya menyimpan data, mengurangi kemungkinan serangan berbasis buffer overflow.

2. **Proteksi terhadap Serangan Buffer Overflow**: Mitigasi seperti _Address Space Layout Randomization_ (ASLR) secara acak menata posisi modul di memori, membuatnya lebih sulit bagi penyerang untuk memprediksi di mana kode mereka akan dieksekusi.

3. **Memperkuat Validasi Memori**: _Control Flow Guard_ (CFG) membantu mencegah serangan yang mencoba memanipulasi alur eksekusi program dengan validasi tambahan pada pemanggilan fungsi.

4. **Proteksi Heap**: Windows mitigations juga mencakup perlindungan pada alokasi memori dinamis (heap) untuk mencegah eksploitasi yang berhubungan dengan manajemen memori.

5. **Mencegah Serangan Privilege Escalation**: Beberapa mitigasi dirancang untuk mencegah proses mendapatkan hak akses lebih tinggi dari yang seharusnya dimiliki, mencegah penyerang mendapatkan kontrol penuh atas sistem.

Windows mitigations secara keseluruhan dirancang untuk meningkatkan ketahanan sistem operasi terhadap eksploitasi yang bisa digunakan oleh malware atau serangan siber.

### Insight Pribadi
- Pengetahuan windows mitigation ini baru bagi saya karena saya belum belajar sama sekali tentang cyber security, jadi untuk mencerna penjelasannya lumayan membuat saya kesulitan.

### Terhubung dengan
- [[buffer overflow]]
- [[alokasi_memori_dinamis]]