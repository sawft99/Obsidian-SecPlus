<%*
let TaskName = await tp.system.prompt("Task name")
let Details = await tp.system.prompt("Details")
let DueDate = await tp.system.prompt("Due date (YYYY-MM-DD)")
let Priority = await tp.system.suggester(["High", "Normal", "Low"], ['<font color="red">High</font>','<font color="White">Normal</font>','<font color="Green">Low</font>'])
if (Details.length != 0) {Details += "<br>"}
-%>
- [ ] <% TaskName %><br><% Details %><sub>Priority: <% Priority %></sub><br><sub>Created: [[<% tp.date.now("YYYY-MM-DD")%>]]</sub><br><sub>Due: [[<% DueDate %>]]</sub>