# Quests
### In Progress
```dataview
LIST
FROM #quests/in-progress
WHERE any(map(file.outlinks, (x) => contains(x.file.path, this.file.folder)))
SORT file.mtime DESCENDING
```
### To Do
```dataview
LIST
FROM #quests/todo
WHERE any(map(file.outlinks, (x) => contains(x.file.path, this.file.folder)))
SORT file.mtime DESCENDING
```
### Complete
```dataview
LIST
FROM #quests/complete
WHERE any(map(file.outlinks, (x) => contains(x.file.path, this.file.folder)))
SORT file.mtime DESCENDING
```
### hooks
```dataview
LIST
FROM #quests/hook
WHERE any(map(file.outlinks, (x) => contains(x.file.path, this.file.folder)))
SORT file.mtime DESCENDING
```