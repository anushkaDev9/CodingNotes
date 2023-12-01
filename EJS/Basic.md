## EJS -Embedded JavaScript
- templating - sending data from server to file then browser.<br/>
- res.sendifle- only for static file<br/>
- render- allows to render the file and add JavaScript objects to pass properties in a key pair value.<br/>
## Install EJS
- npm install express ejs<br/>
## EJS Syntax 
**Basic start - <% %>**<br/>
- **<%= Variable %>** -  JavaScript output<br/>
- **<% console.log(”hello”) %>** - only js code JavaScript Execute (interpreted inside JavaScript file )<br/>
- <%- '<h1>HTML</h1>' %> -Render Html<br/>
- <%% %%>- escape EJS (Ejs tags will be displayed)<br/>
- <%#  this is comment %>- comment<br/>
- <% - include(”filename”) %> - insert another EJS<br/>
## EJS & PASSING DATA
- Locals-way to access all the variables that get sent over. <br/>
- res.local={data:42}
## Partails /Layout
- the files that don’t change <br/>
- app.use(express.static(”public”)<br/>
