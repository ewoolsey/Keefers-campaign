The world has long since been shattered, and now fragments of what remains float in an endless sky known as the Cloud Sea. Large islands, known as [[Shards]] float aimlessly, with large civilizations continuing to thrive upon their surface.

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
- **[[Shards]]**

%% End Waypoint %%