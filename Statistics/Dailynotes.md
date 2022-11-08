
```dataviewjs
dv.list(dv.pages('"Diary"').sort(b => b.file.ctime).map(b => b.file.link));
```
