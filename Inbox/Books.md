---
aliases: 
tags: 
title: Books
date created: Monday, July 18th 2022, 9:56:46 pm
date modified: Monday, August 1st 2022, 10:41:41 pm
---
```dataview
TABLE book, dateformat(file.ctime, "yy-MM-dd") as "Created", dateformat(file.mtime, "yy-MM-dd") as "Last Modified"
  WHERE any(book)
  SORT file.mtime DESC
```

