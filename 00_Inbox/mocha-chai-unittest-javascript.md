
## mocha-chai-unittest-javascript

**tags:** #type/log #topic/programming #topic/javascript #topic/unittest

### Catatan
Saat saya mengerjakan coing di codewars saya binggung code di **Sample Test** itu code javascript apa, dan saya cari melalui chtgpt dan saya tahu itu adalah code unit test utuk javascript, biasanya digunakan oleh codewars yaitu mocha dan chai

saya buat ingin coba menggunakannya tetapi saya ingat mau menggunakan pnpm dibanding npm karena ukuran node_module lebih kecil, akhirnya saya menginstal pnpm dulu
```
npm install -g pnpm
```

dan juga setup pnpm
```
pnpm setup
```

dan saya pun masuk ke folder project saya dan melakukan
```bash
pnpm init

# dan install package mocha dan chai
pnpm add --save-dev mocha chai
```

dan unit test bisa digunakan dengan
```
pnpm mocha nama_file.js
```