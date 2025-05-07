
## Maps of Content: Project

### Aktif
```dataview
LIST
FROM #type/project AND !"99_Templates" AND !"98_Archives"
```

### Idea
```dataview
LIST
FROM #type/projectidea AND !"99_Templates"
```

### Selesai
```dataview
LIST
FROM !"99_Templates" AND "98_Archives" AND #type/project 
```