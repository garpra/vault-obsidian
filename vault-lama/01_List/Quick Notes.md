
#### Back
[[Homepage]]

## Quick Notes List
```dataviewjs
dv.table(["Judul", "Dibuat"], 
  dv.pages('"08_Quick_Notes"')
    .sort(p => p.file.ctime, 'asc')
    .map(p => [
      p.file.link,
      p.file.ctime,
    ])
)

```


