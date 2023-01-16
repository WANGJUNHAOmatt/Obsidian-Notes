---
tags: [DailyNotes]
mood: 
anxiety: 
weight:
sports: 
game:
sex: 0
friend: 0
clock-sleep:
clock-wakeup:
face-washing: 0
tooth-brushing: 0
---

## TimeLog


### 今天新建的文档
```dataview
LIST 
  WHERE file.cday = this.file.day
    and file.name != this.file.name
```

### 今天更新的文档
```dataview
LIST
  WHERE file.mday = this.file.day
    and file.cday != this.file.day
```
