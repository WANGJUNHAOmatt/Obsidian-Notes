---
aliases: 
tags: TOC
date created: Sunday, November 20th 2022, 12:10:04 pm
date modified: Sunday, November 20th 2022, 12:14:24 pm
---

```dataviewjs
dv.header(2, "关于 Python 的内容一览");
var notes = dv.pages("#Programing/Python");
var dateformat = "yyyy-MM-DD";
// dv.list(pages.file.link);
dv.table(
  ["笔记", "创建日期", "最后更新日期"],
  notes.map(x =>
    [
      x.file.link, 
      moment(x.file.ctime.toString()).format(dateformat), 
      moment(x.file.mtime.toString()).format(dateformat)
    ]
  )
);
```
