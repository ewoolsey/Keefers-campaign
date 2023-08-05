# Hooks
### In Progress
```dataview
LIST
FROM #hooks/in-progress
WHERE any(map(file.outlinks, (x) => contains(x.file.path, this.file.folder)))
SORT file.mtime DESCENDING
```
### To Do
```dataview
LIST
FROM #hooks/todo
WHERE any(map(file.outlinks, (x) => contains(x.file.path, this.file.folder)))
SORT file.mtime DESCENDING
```
### Complete
```dataview
LIST
FROM #hooks/complete
WHERE any(map(file.outlinks, (x) => contains(x.file.path, this.file.folder)))
SORT file.mtime DESCENDING
```

<%
	tp.file.move(
		tp.file.path(true).replace(
		tp.file.title + ".md",
		tp.file.title + "/" + tp.file.title
		)
	)
%>

<%* if (true) { %> %% Waypoint %% <%* } %>