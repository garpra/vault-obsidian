
#### Back
[[Homepage]]

> [!quote]
> "Life is like riding a bicycle. To keep your balance, you must keep moving."   -- *Albert Einstein*

### 2025

#### Mei
```dataviewjs
dv.table(["Hari"], 
  dv.pages('"07_Journals/Daily_Journal"')
	.where(p => p.file.cday.month === 5)
    .sort(p => p.file.name, 'desc')
    .map(p => [
      p.file.link
    ])
)
```


#### April
```dataviewjs
dv.table(["Hari"], 
  dv.pages('"07_Journals/Daily_Journal"')
	.where(p => p.file.cday.month === 4)
    .sort(p => p.file.name, 'desc')
    .map(p => [
      p.file.link
    ])
)
```


