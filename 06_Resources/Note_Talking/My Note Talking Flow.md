---
tags:
  - type/note
  - topic/para
  - topic/zettelkasten
  - topic/productivity
---

## My Note Talking Flow

#### 1. 00_Inbox
Menyimpan ide-ide dari project yang akan dibuat nantinya di dalam folder **04_Projects**. Ide yang didapatkan secara spontan misal anda sedang nonton youtube tentang build project, dan anda terpikir untuk membuat projectnya juga tetapi dengan modifikasi anda, maka masukkan ke folder ini. Berikan juga penjelasan ringkas tentang ide projectnya agar lebih mudah memahami idenya di masa depan.

#### 2. 01_Fleetings
Menyimpan ide-ide mentah dan spontan yang terpikirkan, berbeda dari **00_Inbox** ide yang didapatkan di fleeting akan diolah menjadi tulisan bukan project, ide dari fleeting didapatkan dari rasa ingin tahu setelah membaca artikel, menonton youtube, atau tiba-tiba terpikirkan. fleeting yang baik dapat berupa pertanyaan kritis, pertanyaannya bisa digali lebih dalam lagi, dan mudah untuk dikonversi ke Literature atau Permanent Note, contoh Fleeting Note yang baik

> Mengapa banyak orang yang gagal dengan resolusi tahunan? Apa ada cara yang lebih efektif untuk merencanakan resolusi

#### 3. 02_Literatures
Menyimpan tulisan hasil dari membaca artikel atau menonton youtube, hasilnya harus merujuk pada sumber external bukan hasil pemikiran sendiri tetapi ubah hasil tulisannya menggunakan bahasa sendiri yang mudah dipahami agar lebih mudah memahaminya di masa depan, untuk satuiterature note bisa untuk banyak topik, contoh dari literature note

```
---
created: 2025-05-04
source: https://wiki.archlinux.org/title/Wayland
type: literature
---

# Apa Manfaat dari Wayland

Wayland adalah protokol display server modern yang dirancang untuk menggantikan X11. Manfaat utamanya meliputi:

- **Rendering lebih efisien**: Aplikasi bisa menggambar langsung ke tampilan tanpa harus melalui banyak perantara.
- **Keamanan lebih baik**: Wayland membatasi akses aplikasi ke input/output dari aplikasi lain.
- **Simplicity & maintenance**: Kode Wayland lebih bersih dan kecil dibanding X11 yang kompleks dan sudah tua.
- **Lebih smooth & modern**: Karena native support untuk compositing dan frame rate tinggi.

### Refleksi:
Saya baru sadar betapa besarnya kompromi yang terjadi pada X11 demi kompatibilitas. Wayland terasa seperti sistem display yang lebih masuk akal untuk masa depan.

### Potensi Permanent Notes:
- [[Wayland Meningkatkan Keamanan Sistem]]
- [[Arsitektur Wayland Lebih Sederhana dan Modern]]
- [[Wayland Menyediakan Rendering yang Lebih Efisien]]
```

#### 4. 03_Permanents
Menyimpan catatan hasil pemikiran dan pemahaman sendiri yang fokus pada satu ide, harus bisa berdiri sendiri dan tidak perlu konsteks dari luar maksudnya catatannya bisa dipahami tanpa harus mencari lagi artikel yang terkait, biasanya permanent note dibuat setelah membuat Literature Note, dalam satu literature note bisa menciptakan banyak permanent note, contoh dari permanent note setelah memahami literature note diatas

```
---
created: 2025-05-04
type: permanent
---

# Wayland Meningkatkan Keamanan Sistem Dibanding X11

Wayland membatasi aplikasi agar tidak dapat mengakses input dari aplikasi lain, seperti keyboard atau mouse event. Ini mengurangi kemungkinan keylogger atau aktivitas mata-mata lain, yang sangat mungkin di X11 karena setiap aplikasi bisa membaca input global. Ini merupakan lompatan besar dalam arsitektur keamanan sistem desktop.

### Koneksi ke Catatan Lain:
- [[Perbedaan Arsitektur Wayland dan X11]]
- [[Keamanan Desktop Linux]]
```

```
---
created: 2025-05-04
type: permanent
---

# Arsitektur Wayland Lebih Sederhana dan Modern

X11 berkembang selama puluhan tahun dengan banyak patch dan ekstensi. Akibatnya, kode X11 besar, kompleks, dan sulit dirawat. Wayland memulai dari nol, dengan desain lebih minimal dan fokus ke kebutuhan modern. Ini memudahkan pengembang membuat compositor yang lebih ringan dan stabil.

### Koneksi:
- [[Wayland dan Dukungan untuk GPU Modern]]
- [[Simplicity dalam Software Desain]]
```
#### 5. 04_Projects
Menyimpan segala sesuatu hal yang sedang aktif dikerjakan yang memiliki tujuan yang spesifik, catatan harus memiliki hasil akhir yang jelas dan harus bersifat sementara (akan selesai). Isi catatannya bisa bervariasi yang penting relevan dengan project

#### 6. 05_Areas
#### 7. 06_Resources
#### 8. 07_Daily_Journals
