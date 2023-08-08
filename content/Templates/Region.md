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
<%* if (true) { %> %% Waypoint %% <%* } %>