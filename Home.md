# Selamat datang di Vault-ku 👏

> [!quote]
> _"Setiap ide kecil bisa menjadi sesuatu yang besar."_ 

---
### Navigasi
- 📓 [[Daily Journal]]
- 🪧 [[Project]]

### Fleeting Note
```dataview
LIST
FROM "01_Fleetings"
SORT file.mtime asc
LIMIT 5
```

### Area
```dataview
LIST
FROM "05_Areas"
```

---
## Catatan Harian
```dataviewjs
dv.table(["Hari"], 
  dv.pages('"07_Daily_Journals"')
    .sort(p => p.file.name, 'desc')
    .limit(5)
    .map(p => [
      p.file.link
    ])
)
```
