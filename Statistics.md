```dataviewjs
let nofold = '!"10 归档/Template"'
let allFile = dv.pages(nofold).file
let totalMd = "共创建 "+
	allFile.length+" 篇文档"
let totalTag = allFile.etags.distinct().length+" 个标签"
let totalTask = allFile.tasks.length+" 个待办 <br><br>"
dv.paragraph(
	totalMd+"、"+totalTag+"、"+totalTask
)
```