---
<%*
	let title = tp.file.title
	if(title.startsWith("Untitled")){
		title = await tp.system.prompt("Title");
		await tp.file.rename(`${title}`);
	}
	tR += "title: "+`${title}`
%>
created: <%tp.file.creation_date("YYYY-MM-DD HH:mm:ss") %>
---






---
***`=this.file.name`***
***Note Created At:**      `=this.file.ctime`* 
***Note Last Updated At:** `=this.file.mtime`* 
