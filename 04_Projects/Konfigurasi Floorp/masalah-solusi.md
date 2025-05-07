---
tags:
  - topic/linux
  - topic/browser
---

## Masalah Solusi

Untuk dapat menghilangkan link pada pojok kanan bawah buka halaman about: support dan cari Profile Directory pilih Open Directory, Buka folder chrome/ dan edit file userContent.css

Tambahkan code ini pada bagian bawa file
```css
@-moz-document url-prefix(about:home), url-prefix(about:newtab) {
/* CSS code goes here */
  #floorp {
    display: none;
  }
}
```

### Terkait
- [[instalasi-floorp]]
- [[04_Projects/Konfigurasi Floorp/log-dev|log-dev]]
