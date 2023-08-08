### In Progress
```dataview
LIST
FROM #quests/in-progress
SORT file.mtime DESCENDING
```
### To Do
```dataview
LIST
FROM #quests/todo
SORT file.mtime DESCENDING
```
### Complete
```dataview
LIST
FROM #quests/complete
SORT file.mtime DESCENDING
```
### Hooks
```dataview
LIST
FROM #quests/hook 
SORT file.mtime DESCENDING
```
