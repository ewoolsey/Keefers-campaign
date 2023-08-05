[[Gramerai]] is a large island floating within the [[Cloud Sea]]. It was the central point hit by a large winter storm known as the [[Grave Winter]], which brought large amounts of undead soldiers to the island, leaving it uninhabitable. 

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

%% Begin Waypoint %%
- [[Arcane Academy]]
- [[Boney Mire]]
- **[[Candle Stone]]**
- [[Knuckle Mountains]]
- [[Lower Green]]

%% End Waypoint %%