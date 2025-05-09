  

## **Mode dalam Vim**

Vim punya beberapa mode utama:
- **Normal mode**: untuk navigasi dan perintah (default saat buka file)
- **Insert mode**: untuk mengetik teks (`i` untuk masuk)
- **Visual mode**: untuk memilih teks (`v`)
- **Command-line mode**: untuk perintah seperti `:w`, `:q`, dsb

---

## **Navigasi Dasar**

- `h` `j` `k` `l`: gerak kiri, bawah, atas, kanan

- `w`: lompat ke awal kata berikutnya

- `b`: kembali ke awal kata sebelumnya

- `0`: ke awal baris

- `^`: ke awal teks (bukan indent)

- `$`: ke akhir baris

- `gg`: ke awal file

- `G`: ke akhir file

- `:n`: ke baris ke-n

---

## **Masuk ke Insert Mode**

- `i`: sebelum kursor

- `I`: di awal baris

- `a`: setelah kursor

- `A`: di akhir baris

- `o`: baris baru di bawah

- `O`: baris baru di atas

---

## **Editing Teks**

- `x`: hapus karakter di bawah kursor

- `dd`: hapus baris

- `dw`: hapus kata

- `d$`: hapus dari kursor ke akhir baris

- `u`: undo

- `Ctrl + r`: redo

- `yy`: copy baris

- `p`: paste setelah kursor

- `P`: paste sebelum kursor

---

## **Visual Mode**

- `v`: masuk visual mode (karakter)

- `V`: visual mode (baris)

- `Ctrl + v`: visual block (kolom)

- Setelah pilih: `d`, `y`, `p`, dll.

---

## **Pencarian**

- `/kata`: cari ke bawah

- `?kata`: cari ke atas

- `n`: next hasil

- `N`: previous hasil

---

## **Command Mode**

- `:w`: simpan

- `:q`: keluar

- `:wq`: simpan dan keluar

- `:q!`: keluar paksa

- `:e nama_file`: buka file lain

---

## **Trik Umum untuk Coding**

- `%`: lompat ke pasangan tanda kurung

- `.`: ulang perintah terakhir

- `>>`, `<<`: indent kanan/kiri

- `ci"`: hapus isi dalam tanda kutip dan masuk insert mode

- `di(`: hapus isi dalam tanda kurung

---

## **Manipulasi Kata/Kalimat/Blok**

- `ci(`, `ci{`, `ci[`, `ci"`: *Change Inside* tanda kurung/kurawal/quotes (ganti isi dan masuk insert)

- `di'`, `di{`, `di[` dll: *Delete Inside* tanda tersebut

- `yi'`, `yi"`: *Yank Inside* tanda kutip

- `>G`: indent seluruh baris dari kursor ke akhir file

- `=G`: auto-indent seluruh baris dari kursor ke bawah (berguna untuk code formatting)

---

## **Split dan Tab**

- `:vsp filename`: split vertikal

- `:sp filename`: split horizontal

- `Ctrl + w, w`: pindah antar jendela

- `Ctrl + w, h/j/k/l`: arah spesifik antar jendela

- `:tabnew filename`: buka file di tab baru

- `gt` dan `gT`: pindah tab (next dan prev)

---

## **Search & Replace Cepat**

- `:%s/old/new/g`: ganti semua "old" dengan "new"

- `:.,$s/old/new/g`: ganti dari baris sekarang sampai akhir

---

## **Mark dan Jump Cepat**

- `m[a-z]`: tandai posisi (misal `ma` = mark 'a')

- `'a`: lompat ke awal baris di mark 'a'

- `` `a ``: lompat ke posisi kursor di mark 'a'

- `''`: kembali ke posisi sebelumnya

---

## **Clipboard (jika Vim-nya mendukung +clipboard)**

- `"+y`: yank ke clipboard sistem

- `"+p`: paste dari clipboard sistem

---

## **Navigasi Fungsi/Struktur (dengan plugin atau tag)**

- `gd`: *go to definition* (butuh LSP atau ctags)

- `gf`: buka file di bawah kursor

- `K`: lihat dokumentasi (butuh LSP)

---

## **Kombo Cepat dan Efisien**

- `.`: ulang aksi terakhir (super powerful)

- `:%!python3 -m json.tool`: beautify file JSON terbuka

- `:!clang %`: compile file C (misalnya, `:!gcc % -o prog && ./prog`)

---

## **Navigasi Lebih Cepat & Cerdas**

- `*`: cari kata di bawah kursor (maju)

- `#`: cari kata di bawah kursor (mundur)

- `g;` dan `g,`: telusuri undo/redo terakhir

- `{` dan `}`: lompat antar paragraf/blok kode

- `]]` dan `[[`: lompat antar fungsi (dalam file structured seperti Python/C)

---

## **Register & Clipboard**

- `"aY`: yank ke register `a`

- `"ap`: paste dari register `a`

- `:reg`: lihat semua register (termasuk yank sebelumnya)

---

## **Perintah Global (baris spesifik)**

- `:g/pola/`: jalankan perintah untuk semua baris yang cocok

- Contoh: `:g/import/d` → hapus semua baris yang mengandung `import`

---

## **Macro**

- `q[a-z]`: mulai rekam macro ke register tertentu (misal `qa`)

- Jalankan perintah...

- `q`: stop rekam

- `@a`: jalankan macro di register `a`

- `@@`: ulang macro terakhir

---

## **Folding (lipat kode)**

- `zf` lalu gerakkan kursor: buat fold dari blok

- `za`: toggle fold

- `zc` / `zo`: close / open fold

- `:set foldmethod=indent` atau `syntax`: auto fold berdasarkan indentasi atau syntax

---

## **Window Management Cepat**

- `Ctrl + w s`: split horizontal

- `Ctrl + w v`: split vertikal

- `Ctrl + w q`: tutup jendela

- `Ctrl + w =`: samakan ukuran semua jendela

- `Ctrl + w H/J/K/L`: pindah jendela ke kiri/bawah/atas/kanan

---

## **Argument/Text Object**

- `da)` / `ci]`: delete/change *around* tanda kurung

- `vi"` / `va{`: visual select inside/around teks dalam tanda

---

## **Quickfix dan Location List (untuk error/navigation)**

- `:copen` / `:cclose`: buka/tutup quickfix list

- `:cn` / `:cp`: next/prev error atau hasil grep

- `:lopen` / `:lclose`: buka location list (biasanya plugin linting/lsp)

---