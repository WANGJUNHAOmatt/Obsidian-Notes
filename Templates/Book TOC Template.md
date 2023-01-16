---
aliases: 
tags: book_TOC, reading
date begin: 
date end: 
author: 
publisher: 
publish year: 
date created: Wednesday, November 16th 2022, 6:09:17 pm
date modified: Wednesday, November 16th 2022, 6:09:32 pm
---

```dataviewjs
var dateformat = "yyyy-MM-DD";
var notes = dv.pages("#book/book_name");
dv.header(3, "本书相关的笔记");
// dv.list(notes.file.ctime);
dv.table(["笔记名称", "创建日期", "最后更新日期"], notes
  .map(x =>
    [
      x.file.link, 
      moment(x.file.ctime.toString()).format(dateformat), 
      moment(x.file.mtime.toString()).format(dateformat)
    ]
  )
);
```
