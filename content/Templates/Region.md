---
location: [1142.0469, 1208]
mapmarker: Region
---
```dataviewjs
x = await dv.io.load("Templates/Region - Quests.md");
dv.paragraph(x);
```
<%
	tp.file.move(
		tp.file.path(true).replace(
		tp.file.title + ".md",
		tp.file.title + "/" + tp.file.title
		)
	)
%>
# Locations
<%* if (true) { %> %% Waypoint %% <%* } %>