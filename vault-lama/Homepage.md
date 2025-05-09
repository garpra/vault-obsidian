
# Selamat datang di Vault-ku 👏

> [!quote]
> _"Setiap ide kecil bisa menjadi sesuatu yang besar."_ 

---
### Navigasi
- 📓 [[Daily Journal]]
- 💻 [[Programming Project]]
- ⚡️ [[Quick Notes]]
- 📚 [[01_List/Resources|Resources]]

### Fleeting Note
```dataview
LIST
FROM "02_Fleeting"
SORT file.mtime asc
LIMIT 5
```

---
## Catatan Harian
```dataviewjs
dv.table(["Hari"], 
  dv.pages('"07_Journals/Daily_Journal"')
    .sort(p => p.file.ctime, 'desc')
    .limit(5)
    .map(p => [
      p.file.link
    ])
)
```


