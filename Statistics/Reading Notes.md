---
aliases: 
tags: 
title: Reading Notes
date created: Monday, July 18th 2022, 10:29:57 pm
date modified: Monday, August 1st 2022, 10:41:41 pm
---
```dataviewjs
var dateformat = "yyyy-MM-DD";

for (let group of dv.pages().where(p => p.book).groupBy(p => p.book)) 
{ 
  dv.header(3, group.key); 
  dv.table(["Name", "Tags", "Last Modified", "Date Created"],
   group.rows 
     .sort(k => k.ctime, 'desc') 
     .map(k => 
     [
	     k.file.link, 
	     k.file.tags,
	     moment(k.file.mtime.toString()).format(dateformat), 
	     moment(k.file.ctime.toString()).format(dateformat), 
     ])) 
}
```
