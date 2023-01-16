---
aliases: 
tags: book_TOC, reading
date begin: 2022-11-16
date end: 
author: Edward T. Hall
publisher: 上海人民出版社
publish year: 1991
date created: Wednesday, November 16th 2022, 6:09:17 pm
date modified: Wednesday, November 16th 2022, 6:09:32 pm
---

## TOC

1. 时间之声
2. 什么是文化
3. 文化的词汇
4. 基本的三分法
5. 文化即是交流
6. 无处不在的集合
7. 虚幻的元素
8. 有机的模式
9. 时间会说话：美国口音
10. 空间会说话
11. 控制的松弛


```dataviewjs
var dateformat = "yyyy-MM-DD";
var notes = dv.pages("#book/The_Silent_Language");
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
